```
tar
```
---------------------------------
| Acción                 | Comando                                  | Descripción                                                                 |
|------------------------|------------------------------------------|-----------------------------------------------------------------------------|
| **Empaquetar**         | `tar -cvf archivo.tar archivos`          | Crea un archivo `.tar` con los archivos especificados.                     |
| **Visualizar contenido**| `tar -tvf archivo.tar`                  | Muestra el contenido del archivo `.tar` sin extraerlo.                     |
| **Extraer**            | `tar -xvf archivo.tar`                  | Extrae los archivos del archivo `.tar` en el directorio actual.            |
| **Extraer en otro lugar** | `tar -xvf archivo.tar -C destino`      | Extrae los archivos en un directorio diferente especificado por `destino`. |
| **Nota**               | Sin `-C`                                | Si no usas `-C`, los archivos se extraen en el directorio actual.          |

--------------------------------
```
gzip
```
---------------------------------------------------

| Acción                | Comando                      | Descripción                                                                |
|-----------------------|------------------------------|----------------------------------------------------------------------------|
| **Comprimir**         | `gzip ficheros`              | Comprime los archivos especificados; el archivo original desaparece.       |
| **Visualizar**        | `gzip -l archivo.gz`         | Muestra información sobre el archivo comprimido (`.gz`).                   |
| **Descomprimir**      | `gzip -d fichero.gz`         | Descomprime el archivo especificado; el archivo comprimido desaparece.     |
