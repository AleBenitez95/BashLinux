````
nano
````

| Opción               | Descripción                                                                 |
|----------------------|-----------------------------------------------------------------------------|
| `nano archivo`       | Abre el archivo especificado en el editor `nano`. Si el archivo no existe, lo crea. |
| `-c`                 | Muestra la posición del cursor (número de línea y columna) en la parte inferior. |
| `-l`                 | Muestra el número de líneas a la izquierda del texto.                       |
| `-m`                 | Habilita la visualización de los números de línea y columnas.               |
| `-w`                 | Desactiva el ajuste de línea (word wrapping), es decir, las líneas largas no se ajustarán automáticamente. |
| `-b`                 | Muestra la barra de progreso de la carga del archivo.                       |
| `-i`                 | Usa la búsqueda incremental, es decir, busca mientras escribes.            |
| `-v`                 | Muestra la versión de `nano`.                                               |
| `-s`                 | Activa la búsqueda con resaltar (highlight) las coincidencias encontradas. |
| `--help`             | Muestra la ayuda de `nano` con una lista de todas las opciones disponibles. |
| `--tabsize=NUM`      | Establece el tamaño de tabulación (por defecto es 8).                       |
| `--nohelp`           | Inicia `nano` sin mostrar la ayuda al inicio.                              |
| `--cut`              | Habilita el uso del portapapeles del sistema para copiar y pegar texto.     |

----------------------------------------------------------------------------

```
vim
```

| Opción                  | Descripción                                                                 |
|-------------------------|-----------------------------------------------------------------------------|
| `vim archivo`           | Abre el archivo especificado en el editor `vim`. Si el archivo no existe, lo crea. |
| `vim -R archivo`        | Abre el archivo en modo solo lectura (no puedes guardar los cambios).       |
| `vim -b archivo`        | Abre el archivo en modo binario (útil para archivos no-texto).              |
| `vim -u archivo`        | Carga un archivo de configuración específico en lugar del archivo predeterminado de `.vimrc`. |
| `vim --version`         | Muestra la versión de `vim` instalada en el sistema.                        |
| `vim -V`                | Inicia `vim` en modo verbose (muestra información de depuración).           |
| `vim -y archivo`        | Abre el archivo en "modo fácil" (ideal para leer archivos grandes, como logs). |
| `vim --help`            | Muestra la ayuda de `vim` con una lista de opciones disponibles.            |
