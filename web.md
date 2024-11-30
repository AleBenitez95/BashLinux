# Apache2
Instalamos apache2 
```
$sudo apt install apache2
```
El archivo index.html se encuentra en el directorio `/var/www/html/index.html`



| Opción                               | Descripción                                                                 |
|--------------------------------------|-----------------------------------------------------------------------------|
| `apache2`                            | Inicia el servidor Apache2.                                                   |
| `sudo apache2ctl start`              | Inicia el servicio de Apache2.                                                |
| `sudo apache2ctl stop`               | Detiene el servicio de Apache2.                                               |
| `sudo apache2ctl restart`            | Reinicia el servicio de Apache2 (detiene y luego lo inicia).                 |
| `sudo apache2ctl reload`             | Recarga la configuración de Apache2 sin detener el servicio.                 |
| `sudo apache2ctl status`             | Muestra el estado del servicio Apache2.                                       |
| `sudo apache2ctl configtest`         | Verifica la configuración de Apache2 para encontrar errores de sintaxis.      |
| `sudo apache2ctl graceful`           | Realiza una recarga "graciosa", lo que permite que Apache recargue su configuración sin perder conexiones activas. |
| `sudo apache2ctl -V`                 | Muestra la información sobre la versión y configuración de Apache2.          |
| `sudo apache2ctl -M`                 | Muestra una lista de los módulos cargados en Apache2.                         |
| `sudo apache2ctl -t`                 | Verifica la sintaxis de la configuración de Apache2.                          |
| `apache2 -v`                         | Muestra la versión de Apache2 instalada.                                      |
| `apache2 -l`                         | Muestra la lista de los módulos compilados en Apache2.                        |
| `apache2ctl -h`                      | Muestra una lista de todas las opciones disponibles para el comando `apache2ctl`. |
| `sudo service apache2 start`         | Inicia el servicio Apache2 (alternativa a `apache2ctl`).                      |
| `sudo service apache2 stop`          | Detiene el servicio Apache2 (alternativa a `apache2ctl`).                     |
| `sudo service apache2 restart`       | Reinicia el servicio Apache2 (alternativa a `apache2ctl`).                    |
| `sudo service apache2 reload`        | Recarga la configuración de Apache2 sin detener el servicio (alternativa a `apache2ctl reload`). |
| `sudo systemctl start apache2`       | Inicia Apache2 usando `systemd` (en distribuciones que usan `systemd`).       |
| `sudo systemctl stop apache2`        | Detiene Apache2 usando `systemd`.                                             |
| `sudo systemctl restart apache2`     | Reinicia Apache2 usando `systemd`.                                            |
| `sudo systemctl reload apache2`      | Recarga Apache2 usando `systemd`.                                             |
| `sudo systemctl status apache2`      | Muestra el estado del servicio Apache2 usando `systemd`.                      |
