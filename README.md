# Examen 2 - Orquestación de Microservicios

Proyecto de contenerización y orquestación de las APIs de Festivos y Calendario Laboral mediante Docker Compose.

## Arquitectura

La solución está compuesta por cuatro contenedores principales:

- MongoDB: base de datos de la API de Festivos.
- API Festivos: microservicio desarrollado con Node.js.
- PostgreSQL: base de datos de la API de Calendario.
- API Calendario: microservicio desarrollado con Spring Boot.

Los servicios se comunican mediante una red Docker tipo bridge denominada `redcalendario`.

## Estructura

- `apiFestivos/` — API de Festivos.
- `apiCalendario/` — API de Calendario Laboral.
- `bdFestivos/` — configuración e inicialización de MongoDB.
- `bdCalendario/` — configuración e inicialización de PostgreSQL.
- `docker-compose.yml` — orquestación de todos los servicios.

## Ejecución

Requisitos:

- Docker Desktop
- Docker Compose

Para construir y levantar los servicios:

```powershell
docker compose up -d --build