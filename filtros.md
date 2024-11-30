```
$pr
```
| Opción                 | Descripción                                                                |
|------------------------|----------------------------------------------------------------------------|
| `pr [opciones] fichero`| Da formato a un archivo de texto para la impresión o visualización.         |
| `pr -h "texto"`         | Añade un título en la parte superior de la salida. Ejemplo: `-h "Informe"`. |
| `pr -d`                 | Usa doble espacio entre las líneas.                                         |
| `pr -w nº`              | Define el ancho de la página en número de caracteres. Ejemplo: `-w 80`.     |
| `pr -l nº`              | Define la longitud de la página en número de líneas. Ejemplo: `-l 50`.      |
| `pr -n`                 | Añade números de línea a la salida.                                         |
| `pr -t`                 | No muestra la cabecera ni los números de página en la salida.              |
| `pr -s "caracter"`      | Especifica un carácter para separar las columnas de salida.                |
| `pr -f`                 | Imprime las páginas del archivo sin encabezado ni título.                  |
| `comando | pr`          | Pasa la salida de un comando al formato `pr` para dar formato a la salida.  |

```
$sort
```
| Opción                       | Descripción                                                                |
|------------------------------|----------------------------------------------------------------------------|
| `sort [opciones] fichero`     | Ordena el contenido del archivo o los archivos especificados.              |
| `sort -n`                     | Realiza una ordenación numérica en lugar de la alfabética por defecto.     |
| `sort -u`                     | Elimina las líneas repetidas en la salida.                                 |
| `comando | sort [opciones]`    | Pasa la salida de un comando al comando `sort` para ordenar los resultados. |
| `sort -t "separador" -k n`    | Ordena el archivo especificando un separador de campos y el campo a ordenar. |
| `sort -t, -k2 fichero`        | Ordena el archivo usando la coma `,` como separador y el campo 2 como clave de ordenación. |
| `sort -t: -k2,4 fichero`      | Ordena el archivo usando `:` como separador y los campos 2, 3 y 4 para ordenar. |
| `sort -t: -k2 -k4 fichero`    | Ordena primero por el campo 2, luego por el campo 4, usando `:` como separador. |

```
$tr
```
| Opción                      | Descripción                                                                |
|-----------------------------|----------------------------------------------------------------------------|
| `tr [opciones] conj1 conj2` | Sustituye los caracteres en `conj1` por los caracteres correspondientes en `conj2`. |
| `comando | tr [opciones] conj1 conj2` | Aplica el comando `tr` sobre la salida de otro comando.                    |
| `tr -s`                      | Sustituye conjuntos de caracteres repetidos por un solo carácter.         |
| `tr -c`                      | Sustituye todos los caracteres **que no** estén en `conj1` por los caracteres en `conj2`. |
| `tr -d`                      | Elimina los caracteres que se encuentren en `conj1`.                      |

```
$sed
```
| Opción                   | Descripción                                                                |
|--------------------------|----------------------------------------------------------------------------|
| `sed 's/cadena1/cadena2/' fichero` | Sustituye la primera aparición de `cadena1` por `cadena2` en cada línea del archivo. |
| `sed 's/cadena1/cadena2/g' fichero` | Sustituye **todas** las apariciones de `cadena1` por `cadena2` en cada línea del archivo. |
| `sed -i 's/cadena1/cadena2/' fichero` | Realiza la sustitución **en el archivo** directamente (sin crear una copia). |
| `sed 's/cadena1/cadena2/2' fichero` | Sustituye solo la **segunda** aparición de `cadena1` por `cadena2` en cada línea. |
| `sed 's/cadena1/cadena2/3g' fichero` | Sustituye solo la tercera aparición de `cadena1` por `cadena2` en cada línea. |
| `sed 's/cadena1/cadena2/p' fichero` | Imprime solo las líneas que han sido modificadas por la sustitución. |
| `sed -n 's/cadena1/cadena2/p' fichero` | **Solo muestra** las líneas donde se ha realizado la sustitución. |
| `sed 's/cadena1/cadena2/'` | Se puede usar sin archivo, para trabajar directamente con la entrada estándar (p. ej., con un `echo` o un pipe). |

```
$grep
```
| Opción                    | Descripción                                                                |
|---------------------------|----------------------------------------------------------------------------|
| `grep [opciones] patrón fichero` | Busca el patrón en el archivo o archivos especificados.                    |
| `grep -i`                  | Ignora las diferencias entre mayúsculas y minúsculas al buscar.            |
| `grep -v`                  | Devuelve las líneas que **no** contienen el patrón.                        |
| `grep -c`                  | Cuenta el número de líneas en las que se ha encontrado el patrón.         |
| `grep -r`                  | Busca recursivamente en todos los archivos dentro de un directorio.       |
| `grep "cadena"`            | Utiliza comillas para especificar el patrón a buscar.                      |
| `grep "^cadena"`           | Busca las líneas que **comienzan** con la cadena especificada.            |
| `grep "cadena$"`           | Busca las líneas que **terminan** con la cadena especificada.             |
| `grep "."`                 | Representa cualquier carácter.                                            |
| `grep ".*"`                | Representa cualquier secuencia de caracteres (cero o más).                 |

```
$cut
```
| Opción                     | Descripción                                                               |
|----------------------------|---------------------------------------------------------------------------|
| `cut -d [separador] -f [campos] fichero` | Selecciona los campos especificados en el archivo, utilizando un delimitador. |
| `-d`                        | Especifica el delimitador de campos.                                      |
| `-f`                        | Especifica qué campos (columnas) extraer. Puede ser un campo único o un rango de campos. |
| `-f1,3,5`                   | Selecciona los campos 1, 3 y 5.                                           |
| `-f3-5`                     | Selecciona los campos 3, 4 y 5.                                           |
| `-d ' '`                    | Utiliza el espacio como delimitador entre campos.                         |
| `-d ':'`                    | Utiliza el carácter `:` como delimitador entre campos.                    |
| `-d $'\t'`                  | Utiliza el tabulador como delimitador (específico para tabuladores).      |
| `cat fichero | cut -d ':' -f 1,3,5` | Extrae los campos 1, 3 y 5 de cada línea de `fichero`, usando `:` como delimitador. |
| `cat fichero | cut -d ' ' -f 3-5` | Extrae los campos 3, 4 y 5 de cada línea de `fichero`, usando espacio como delimitador. |

```
$paste
```
| Opción                         | Descripción                                                                |
|--------------------------------|----------------------------------------------------------------------------|
| `paste [opciones] fichero1 fichero2` | Une los archivos especificados línea por línea.                            |
| `-d`                           | Especifica el **separador** que se usará entre las columnas. Por defecto, se utiliza el tabulador. |
| `-d <separador>`               | Permite definir el separador entre los archivos unidos. Puedes usar comas, espacios u otros caracteres. |

````
$awk
````
| Opción                         | Descripción                                                               |
|--------------------------------|---------------------------------------------------------------------------|
| `awk -F <separador> '{condición} {orden}' fichero` | Extrae y procesa información de un archivo, usando un delimitador (`-F`) y especificando una condición y orden. |
| `-F <separador>`               | Define el **separador** de campos. Por defecto es el espacio o tabulador, pero se puede especificar otro delimitador, como `:`. |
| `{print $n}`                   | Imprime el campo **n** del archivo, donde `n` es el número del campo. |
| `{print $0}`                   | Imprime toda la línea (todos los campos).                               |
| `$n`                           | Se refiere al campo número **n** en la línea.                            |
| `&&`                           | Operador lógico **Y** (AND).                                              |
| `||`                           | Operador lógico **OR** (O).                                               |
| `$1 == valor`                  | Condición que verifica si el primer campo (`$1`) es igual a un valor.   |
| `$1 != valor`                  | Condición que verifica si el primer campo (`$1`) es diferente de un valor. |
| `$n > valor`                   | Condición que verifica si el campo **n** es mayor que un valor.         |
| `$n <= valor`                  | Condición que verifica si el campo **n** es menor o igual que un valor. |

```
$join
```
| Opción                         | Descripción                                                               |
|--------------------------------|---------------------------------------------------------------------------|
| `join -t <delimitador> -1 <campo1> -2 <campo2> fichero1 fichero2` | Une los datos de dos ficheros usando un campo común. `-t` especifica el delimitador, `-1` es el campo común en el primer fichero y `-2` es el campo común en el segundo fichero. |
| `-t <delimitador>`             | Especifica el delimitador utilizado para separar los campos en los ficheros. Si no se indica, el delimitador predeterminado es el espacio o tabulador. |
| `-1 <campo1>`                 | Define el campo en el primer fichero que se utilizará como clave para realizar la unión. |
| `-2 <campo2>`                 | Define el campo en el segundo fichero que se utilizará como clave para realizar la unión. |

