```
ssh
```
| Opción                                | Descripción                                                                 |
|---------------------------------------|-----------------------------------------------------------------------------|
| `ssh usuario@servidor`                | Conecta al servidor remoto como el usuario especificado.                    |
| `ssh -l usuario servidor`             | Conecta al servidor remoto como el usuario especificado, usando la opción `-l` para el login. |
| `ssh -p puerto usuario@servidor`      | Especifica el puerto de conexión (por defecto es el puerto 22).              |
| `ssh -v usuario@servidor`             | Muestra información detallada de la conexión para depuración (modo verbose). |
| `ssh -vv usuario@servidor`            | Muestra más información detallada que con la opción `-v`.                    |
| `ssh -vvv usuario@servidor`           | Muestra la máxima cantidad de información de depuración (modo ultra verbose).|
| `ssh -i archivo.pem usuario@servidor` | Especifica una clave privada para la autenticación (archivo PEM).            |
| `ssh -X usuario@servidor`             | Permite la ejecución de aplicaciones gráficas a través de SSH (X forwarding).|
| `ssh -Y usuario@servidor`             | Habilita el "trusted X forwarding", que es menos restrictivo que `-X`.       |
| `ssh -o "Opción=valor" usuario@servidor` | Permite especificar opciones adicionales de configuración en línea (por ejemplo, `-o "StrictHostKeyChecking=no"`). |
| `ssh -f usuario@servidor`             | Ejecuta el comando en segundo plano después de la autenticación.             |
| `ssh -N usuario@servidor`             | No ejecuta ningún comando, solo establece la conexión SSH.                    |
| `ssh -T usuario@servidor`             | No asigna pseudo-terminal (para conexiones no interactivas, como las de Git).|
| `ssh -C usuario@servidor`             | Habilita la compresión de datos durante la conexión.                         |
| `ssh -A usuario@servidor`             | Habilita el reenvío de agentes SSH (permitiendo el uso de claves SSH a través de saltos de host).|
| `ssh -E archivo.log usuario@servidor` | Registra la salida de la sesión SSH en el archivo especificado.              |
| `ssh usuario@servidor "comando"`      | Ejecuta un comando remoto sin iniciar una sesión interactiva.                |
| `ssh usuario@servidor -T "comando"`   | Ejecuta un comando remoto sin asignar un terminal, útil para scripts.        |
| `ssh-keygen`                          | Crea una nueva clave SSH.                                                   |
| `ssh-copy-id usuario@servidor`        | Copia la clave pública SSH al servidor remoto para permitir el acceso sin contraseña. |
| `ssh -Q key-types`                    | Muestra los tipos de claves soportados.                                      |
| `ssh -Q cipher`                       | Muestra los cifrados soportados por el servidor SSH.                         |
| `ssh -Q mac`                          | Muestra los algoritmos de MAC soportados.                                    |
| `ssh -Q hostkey`                      | Muestra los algoritmos de clave de host soportados.                          |
| `ssh-add`                             | Añade claves privadas al agente SSH para facilitar la autenticación sin contraseña. |
| `ssh-agent`                           | Inicia un agente SSH para manejar claves privadas.                          |
| `ssh -K`                              | Desactiva el reenvío de agentes SSH.                                         |
| `ssh -L [puerto_local]:[host_remoto]:[puerto_remoto] usuario@servidor` | Crea un túnel SSH local, redirigiendo el tráfico de un puerto local a un puerto remoto. |
| `ssh -R [puerto_remoto]:[host_local]:[puerto_local] usuario@servidor` | Crea un túnel SSH remoto, redirigiendo el tráfico de un puerto remoto a un puerto local. |
