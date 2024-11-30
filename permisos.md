```
chmod [opciones] permisos archivo
```

### Modo simbólico

| Símbolo | Significado                               |
|---------|-------------------------------------------|
| `u`     | Usuario (propietario del archivo)         |
| `g`     | Grupo (usuarios en el mismo grupo)        |
| `o`     | Otros (resto de los usuarios)            |
| `a`     | Todos (`u`, `g`, y `o`)                  |
| `+`     | Añadir permiso                            |
| `-`     | Quitar permiso                            |
| `=`     | Asignar permisos exactos (reemplaza todos)|


### Modo numérico

| Permiso              | Número |
|----------------------|--------|
| Sin permisos         | 0      |
| Solo ejecución       | 1      |
| Solo escritura       | 2      |
| Escritura y ejecución| 3      |
| Solo lectura         | 4      |
| Lectura y ejecución  | 5      |
| Lectura y escritura  | 6      |
| Todos los permisos   | 7      |
