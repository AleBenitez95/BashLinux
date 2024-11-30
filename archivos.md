```
ls
```

| Opción               | Descripción                                                   |
|----------------------|---------------------------------------------------------------|
| `-a`                | Muestra todos los archivos, incluidos los ocultos (comienzan con `.`). |
| `-A`                | Similar a `-a`, pero excluye `.` (directorio actual) y `..` (directorio padre). |
| `-l`                | Lista en formato detallado, mostrando permisos, propietario, tamaño, etc. |
| `-h`                | Muestra tamaños en un formato legible para humanos (KB, MB, etc.). Se usa con `-l`. |
| `-R`                | Lista contenido de directorios recursivamente. |
| `-t`                | Ordena los archivos por fecha de modificación (más reciente primero). |
| `-r`                | Invierte el orden de la lista (ej., alfabetización descendente). |
| `-S`                | Ordena los archivos por tamaño, de mayor a menor. |
| `-1`                | Muestra un archivo o directorio por línea. |
| `-d`                | Lista directorios en lugar de su contenido. |
| `-i`                | Muestra el número de inodo para cada archivo. |
| `-F`                | Añade un indicador al final de los nombres de archivos (ej., `/` para directorios). |
| `-G`                | Usa colores para distinguir tipos de archivos (si está habilitado). |
| `--color`           | Forza o desactiva el color en la salida (valores: `always`, `auto`, `never`). |
| `--full-time`       | Muestra fechas y horas completas en el listado. |
| `-n`                | Muestra los IDs numéricos de usuario y grupo en lugar de sus nombres. |
| `-p`                | Añade `/` a los nombres de directorios. |
| `--sort=[TYPE]`     | Especifica el tipo de ordenación (`name`, `size`, `time`, `extension`). |
| `-X`                | Ordena por extensión de archivo. |
| `-v`                | Ordena por versión (útil para nombres con números, como `file1`, `file2`). |
| `--hide=[PATTERN]`  | Oculta archivos que coincidan con un patrón especificado. |
| `--help`            | Muestra la ayuda del comando `ls`. |
| `--version`         | Muestra la versión del comando `ls`. |
