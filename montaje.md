# Montaje

| Comando                | Opción                          | Descripción |
|------------------------|---------------------------------|-------------|
| `fdisk -l`             | N/A                             | Muestra las particiones de los discos duros y el nombre asignado a cada dispositivo. |
| `mount`                | `-o`                            | Especifica opciones adicionales, como la lectura/escritura o el acceso exclusivo. Ejemplo: `-o ro` para solo lectura. |
|                        | `-t tipo`                       | Especifica el tipo de sistema de archivos (ej. `ext4`, `ntfs`, `vfat`, etc.). |
| `umount`               | N/A                             | Desmonta un dispositivo o punto de montaje. Ejemplo: `umount /dev/sdb1` o `umount /media/cdrom`. |
| `df`                   | `-h`                            | Muestra el espacio en disco de manera legible para humanos (en MB/GB). |
|                        | `-T`                            | Muestra el tipo de sistema de archivos junto con la información de uso del disco. |
| `lsblk`                | `-f`                            | Muestra información sobre dispositivos de bloques con sus sistemas de archivos. |
| `eject`                | N/A                             | Expulsa un dispositivo (como un CD/DVD) o desmonta el dispositivo si está montado. |
| `lsof +D`              | N/A                             | Lista los archivos abiertos de un directorio. Puede ayudar a identificar procesos que están usando un dispositivo montado. |
| `cat`                  | N/A                             | Puede usarse para crear una imagen ISO de un dispositivo. Ejemplo: `cat /dev/hdc > imagen.iso`. |
| `mount -o loop`        | N/A                             | Monta una imagen ISO como si fuera un dispositivo. Ejemplo: `mount -o loop imagen.iso /media/iso`. |
| `mount -a`             | N/A                             | Monta todos los sistemas de archivos listados en el archivo `/etc/fstab` sin necesidad de reiniciar. |
| `blkid`                | N/A                             | Muestra el UUID y otros detalles sobre los dispositivos. Útil para agregar entradas en `/etc/fstab`. |
