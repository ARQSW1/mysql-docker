# MYSQL CON DOCKER COMPOSE

El proyecto realiza el despliegue de una solucion con los siguientes componentes

![ARQUITECTURA](./doc/arch.drawio.svg)


- **MYSQL**: Motor de base de datos *Open Source* .
    - Usuario: `root`
    - Contraseña: `example`
- **PhpMyAdmin**: UI Web de administración de MySQL
    - URL : http://admin.localdev.me:8001
    - Usuario: `root`
    - Contraseña: `example`

## Archivos

- `docker-compose.yaml` implementación declarativa de la solución
- `doc` documentación del sistema

## Utilización

Para iniciar 

```bash
docker compose --project-name mysql up -d
```


# Eliminar 

Elimina los contenedores pero conserva el volumen
```bash
docker compose --project-name mysql down
```

Elimina todo
```bash
docker compose --project-name mysql down -v
```
