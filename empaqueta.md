-------------------------------------------
```
$tar
```

| Acción                 | Comando                                  | Descripción                                                                 |
|------------------------|------------------------------------------|-----------------------------------------------------------------------------|
| **Empaquetar**         | `tar -cvf archivo.tar archivos`          | Crea un archivo `.tar` con los archivos especificados.                     |
| **Visualizar contenido**| `tar -tvf archivo.tar`                  | Muestra el contenido del archivo `.tar` sin extraerlo.                     |
| **Extraer**            | `tar -xvf archivo.tar`                  | Extrae los archivos del archivo `.tar` en el directorio actual.            |
| **Extraer en otro lugar** | `tar -xvf archivo.tar -C destino`      | Extrae los archivos en un directorio diferente especificado por `destino`. |
| **Nota**               | Sin `-C`                                | Si no usas `-C`, los archivos se extraen en el directorio actual.          |

--------------------------------
```
$gzip
```


| Acción                | Comando                      | Descripción                                                                |
|-----------------------|------------------------------|----------------------------------------------------------------------------|
| **Comprimir**         | `gzip ficheros`              | Comprime los archivos especificados; el archivo original desaparece.       |
| **Visualizar**        | `gzip -l archivo.gz`         | Muestra información sobre el archivo comprimido (`.gz`).                   |
| **Descomprimir**      | `gzip -d fichero.gz`         | Descomprime el archivo especificado; el archivo comprimido desaparece.     |

------------------------------------------

```
$zip
```
| Acción                | Comando                             | Descripción                                                                |
|-----------------------|-------------------------------------|----------------------------------------------------------------------------|
| **Comprimir**         | `zip archivo.zip ficheros_a_comprimir` | Comprime los archivos especificados en un archivo `.zip`.                 |
| **Visualizar**        | `unzip -v archivo.zip`              | Muestra información sobre el archivo comprimido `.zip`.                    |
| **Descomprimir**      | `unzip archivo.zip -d Directorio_destino` | Extrae el contenido del archivo `.zip` en el directorio especificado.    |


----------------------------------------------

```
$bzip2
```

| Acción                | Comando                            | Descripción                                                                |
|-----------------------|------------------------------------|----------------------------------------------------------------------------|
| **Comprimir**         | `bzip2 ficheros`                   | Comprime los archivos especificados en un archivo `.bz2`; el archivo original desaparece. |
| **Visualizar**        | `bzip2 -v archivo.bz2`             | Muestra información sobre el archivo comprimido `.bz2`.                    |
| **Descomprimir**      | `bzip2 -d fichero.bz2`             | Descomprime el archivo `.bz2`; el archivo comprimido desaparece.           |

----------------------------------------------------

```
%.tar.gz
```

| Acción                      | Comando                                | Descripción                                                                |
|-----------------------------|----------------------------------------|----------------------------------------------------------------------------|
| **Empaquetar y comprimir**   | `tar -zcvf archivo.tar.gz archivos_origen` | Empaqueta y comprime los archivos en un archivo `.tar.gz`.                |
| **Visualizar**               | `tar -ztvf archivo.tar.gz`             | Muestra el contenido de un archivo `.tar.gz` sin extraerlo.                |
| **Descomprimir y desempaquetar** | `tar -zxvf archivo.tar.gz -C destino`  | Descomprime y desempaqueta los archivos en el directorio especificado por `destino`. |
| **Nota sobre `-C`**          | Sin `-C`                              | Si no usas `-C`, los archivos se extraen en el directorio actual.          |

----------------------------------------------------------------

```
%-tar.bz2
```
| Acción                      | Comando                                | Descripción                                                                |
|-----------------------------|----------------------------------------|----------------------------------------------------------------------------|
| **Empaquetar y comprimir**   | `tar -jcvf archivo.tar.bz2 archivos_origen` | Empaqueta y comprime los archivos en un archivo `.tar.bz2`.                |
| **Visualizar**               | `tar -jtvf archivo.tar.bz2`            | Muestra el contenido de un archivo `.tar.bz2` sin extraerlo.               |
| **Descomprimir y desempaquetar** | `tar -jxvf archivo.tar.bz2 -C destino` | Descomprime y desempaqueta los archivos en el directorio especificado por `destino`. |
| **Nota sobre `-C`**          | Sin `-C`                              | Si no usas `-C`, los archivos se extraen en el directorio actual.          |


