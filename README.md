# Nexo Solar — descargas

Instaladores publicados de **Nexo Solar**, el software del banco de pruebas
solar y meteorológico del SENA CIDT de Barrancabermeja.

Este repositorio **no contiene el código fuente**: solo sirve las descargas.
Cada versión se publica desde el repositorio privado del proyecto, y solo
después de que el instalador se compiló, se instaló y se probó de forma
automática en Windows y en Fedora.

## Descargar

Las versiones están en la página de [Releases](../../releases).

| Sistema | Archivo |
|---|---|
| Windows 10 y 11 (64 bits) | `NexoSolar-<versión>-windows-x64-setup.exe` |
| Fedora 43 y 44 (x86_64) | `nexo-solar-<versión>-1.x86_64.rpm` |

## Verificar la descarga

Cada versión publica un archivo `SHA256SUMS.txt`. Antes de instalar, comprobá
que el archivo llegó completo: una descarga o una copia a un USB que se
interrumpe deja un archivo corrupto que el sistema rechaza al ejecutarlo.

En Windows, con PowerShell:

    Get-FileHash .\NexoSolar-<versión>-windows-x64-setup.exe -Algorithm SHA256

En Fedora:

    sha256sum -c SHA256SUMS.txt

El valor debe coincidir exactamente con el publicado en la versión.

## Licencia

El software se distribuye bajo licencia de uso restringido. Los avisos de
licencia de los componentes de terceros viajan dentro del propio instalador.
