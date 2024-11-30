# Información del Comando `nmap`

| **Categoría**             | **Opción**                          | **Descripción**                                                                                     |
|---------------------------|-------------------------------------|-----------------------------------------------------------------------------------------------------|
| **Descubrimiento de hosts** | `-sn`                              | Escaneo sin puerto, solo identifica dispositivos activos (ping scan).                              |
|                           | `-sP`                              | Similar a `-sn`, verifica qué dispositivos responden.                                              |
| **Escaneo de puertos**     | `-sT`                              | Escaneo TCP (conexión completa).                                                                   |
|                           | `-sS`                              | Escaneo TCP SYN (semi-abierto).                                                                    |
|                           | `-sU`                              | Escaneo de puertos UDP.                                                                            |
|                           | `-p [puertos]`                     | Especifica puertos a escanear, por ejemplo, `-p 22,80,443` o `-p 1-65535`.                         |
| **Detección de servicios y sistemas** | `-sV`                              | Detecta versiones de servicios.                                                                    |
|                           | `-O`                               | Detecta el sistema operativo.                                                                      |
|                           | `-A`                               | Escaneo avanzado (OS, servicios y traza de red).                                                  |
| **Salida personalizada**   | `-oN [archivo]`                    | Salida en formato normal.                                                                          |
|                           | `-oX [archivo]`                    | Salida en formato XML.                                                                             |
|                           | `-oG [archivo]`                    | Salida en formato "grepable".                                                                      |
|                           | `-v`                               | Modo verboso.                                                                                      |
|                           | `-vv`                              | Modo muy verboso.                                                                                  |
| **Escaneo sigiloso**       | `-T[0-5]`                          | Controla la agresividad del escaneo (0 = más sigiloso, 5 = más rápido).                            |
|                           | `-Pn`                              | Evita realizar un ping previo al escaneo.                                                          |
| **Scripts NSE**            | `--script=[nombre del script]`     | Ejecuta scripts específicos.                                                                       |
|                           | `--script-help=[nombre del script]`| Muestra información sobre un script.                                                               |

---

## Ejemplo práctico

| **Comando**                                  | **Descripción**                                                                                  |
|---------------------------------------------|--------------------------------------------------------------------------------------------------|
| `nmap -sS -p 80,443 -O -v 192.168.1.1`       | Escaneo SYN de puertos 80 y 443, detecta sistema operativo, en modo verboso.                    |
| `nmap --script vuln 192.168.1.1`             | Ejecuta un script de vulnerabilidades contra el host 192.168.1.1.                               |
