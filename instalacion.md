```
$sudo apt
```
| Opción                        | Descripción                                                               |
|-------------------------------|---------------------------------------------------------------------------|
| `apt`                          | Interfaz de línea de comandos para la gestión de paquetes.                |
| `apt update`                   | Actualiza la lista de paquetes disponibles desde los repositorios configurados. |
| `apt upgrade`                  | Actualiza todos los paquetes instalados a su versión más reciente.        |
| `apt full-upgrade`             | Realiza una actualización más completa, eliminando o instalando nuevos paquetes si es necesario. |
| `apt install <paquete>`        | Instala un paquete especificado.                                          |
| `apt remove <paquete>`         | Elimina un paquete, pero deja los archivos de configuración.              |
| `apt purge <paquete>`          | Elimina un paquete y sus archivos de configuración.                       |
| `apt autoremove`               | Elimina paquetes que fueron instalados automáticamente como dependencias y que ya no son necesarios. |
| `apt search <paquete>`         | Busca un paquete en los repositorios disponibles.                         |
| `apt show <paquete>`           | Muestra información detallada sobre un paquete (como versión, dependencias, etc.). |
| `apt list --installed`         | Muestra una lista de todos los paquetes instalados.                       |
| `apt list <paquete>`           | Muestra información sobre un paquete específico, si está disponible.     |
| `apt-cache search <paquete>`   | Busca un paquete en los repositorios sin instalarlo (usado en versiones antiguas de apt). |
| `apt-cache show <paquete>`     | Muestra detalles de un paquete sin necesidad de instalarlo (antiguo).    |
| `apt autoremove`               | Elimina paquetes innecesarios que ya no son requeridos por otros paquetes. |
| `apt clean`                    | Limpia el caché local de paquetes descargados (elimina archivos `.deb` almacenados). |
| `apt purge`                    | Elimina un paquete y todos sus archivos de configuración.                |
| `apt edit-sources`             | Abre el archivo de fuentes de software (`/etc/apt/sources.list`) en un editor de texto para su edición. |

```
$dpkg
```
| Opción                        | Descripción                                                               |
|-------------------------------|---------------------------------------------------------------------------|
| `dpkg`                         | Herramienta de bajo nivel para gestionar paquetes en formato `.deb`.      |
| `dpkg -i <paquete.deb>`        | Instala el paquete especificado en formato `.deb`.                        |
| `dpkg -r <paquete>`            | Elimina el paquete especificado, pero conserva sus archivos de configuración. |
| `dpkg --remove <paquete>`      | Elimina el paquete especificado, pero conserva sus archivos de configuración. |
| `dpkg -P <paquete>`            | Elimina el paquete especificado y sus archivos de configuración.         |
| `dpkg --purge <paquete>`       | Elimina el paquete y sus archivos de configuración.                       |
| `dpkg -l`                      | Muestra una lista de todos los paquetes instalados en el sistema.         |
| `dpkg -L <paquete>`            | Muestra los archivos instalados por un paquete especificado.             |
| `dpkg -s <paquete>`            | Muestra información detallada sobre un paquete instalado.                |
| `dpkg --get-selections`        | Muestra el estado de los paquetes instalados (por ejemplo, si están instalados o no). |
| `dpkg --set-selections`        | Permite cambiar el estado de los paquetes (por ejemplo, marcar paquetes para ser instalados o eliminados). |
| `dpkg -S <archivo>`            | Busca el paquete al que pertenece un archivo específico.                 |
| `dpkg --configure <paquete>`   | Configura un paquete que ha sido descomprimido pero no ha sido configurado. |
| `dpkg --audit`                 | Muestra los paquetes que están en un estado inconsistente (por ejemplo, paquetes parcialmente instalados). |
| `dpkg --listfiles <paquete>`   | Muestra los archivos de un paquete específico instalado en el sistema.   |
