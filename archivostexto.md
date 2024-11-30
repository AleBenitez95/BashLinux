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

| Acción                           | Comando en Vim                        | Descripción                                                                |
|----------------------------------|---------------------------------------|----------------------------------------------------------------------------|
| **Abrir archivo**                | `vim archivo`                         | Abre el archivo en `vim`. Si no existe, crea un archivo nuevo.              |
| **Entrar en modo de inserción**  | `i`                                   | Entra en el modo de inserción para empezar a escribir.                     |
| **Volver al modo de comando**    | `Esc`                                 | Sale del modo de inserción y vuelve al modo de comando.                    |
| **Guardar archivo**              | `:w`                                  | Guarda los cambios del archivo actual.                                     |
| **Salir de Vim**                 | `:q`                                  | Sale de Vim. Si hay cambios sin guardar, te pedirá confirmación.           |
| **Guardar y salir**              | `:wq`                                 | Guarda los cambios y luego sale de Vim.                                    |
| **Salir sin guardar cambios**    | `:q!`                                 | Sale sin guardar los cambios.                                              |
| **Borrar una línea**             | `dd`                                  | Borra la línea donde está el cursor.                                       |
| **Copiar una línea**             | `yy`                                  | Copia la línea donde está el cursor.                                       |
| **Pegar texto**                  | `p`                                   | Pega el texto copiado o cortado después del cursor.                        |
| **Deshacer cambio**              | `u`                                   | Deshace el último cambio realizado.                                        |
| **Rehacer cambio**               | `Ctrl + r`                            | Rehace el cambio que fue deshecho.                                         |
| **Buscar texto**                 | `/texto`                              | Busca el texto especificado hacia adelante.                                |
| **Buscar hacia atrás**           | `?texto`                              | Busca el texto especificado hacia atrás.                                   |
| **Moverse al inicio del archivo**| `gg`                                  | Mueve el cursor al principio del archivo.                                  |
| **Moverse al final del archivo** | `G`                                   | Mueve el cursor al final del archivo.                                      |
| **Ir a una línea específica**    | `:n`                                  | Mueve el cursor a la línea número `n`.                                     |
| **Moverse al inicio de una línea**| `0`                                  | Mueve el cursor al inicio de la línea actual.                              |
| **Moverse al final de una línea**| `$`                                  | Mueve el cursor al final de la línea actual.                               |
| **Reemplazar texto**             | `r` seguido de un carácter            | Reemplaza el carácter bajo el cursor por el que se especifique.            |
| **Abrir otra ventana (archivo)** | `:e otro_archivo`                     | Abre un archivo diferente en la misma sesión de Vim.                       |
| **Dividir la ventana**           | `:split`                              | Divide la ventana de Vim en dos.                                           |
| **Cerrar la ventana actual**     | `:q`                                  | Cierra la ventana actual (si hay varias ventanas abiertas).                |


