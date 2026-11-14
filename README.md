
# Sistema de Reserva de Horas Medicas

## Proyecto DevOps - IACC 2026

Aplicacion web estatica que simula un sistema
de reserva de horas medicas para una empresa
del sector salud.

## Objetivo

Aplicar practicas DevOps utilizando Git, GitHub,
Docker Desktop, Docker Compose y Nginx.

## Tecnologias utilizadas

- HTML5 y CSS3
- Visual Studio Code
- Git y GitHub
- Docker Desktop
- Docker Compose
- Nginx Alpine

## Estructura del proyecto

- src/index.html: interfaz del formulario medico.
- src/styles.css: estilos de la aplicacion.
- Dockerfile: construccion de la imagen.
- docker-compose.yml: configuracion del servicio.
- .gitignore: exclusion de archivos privados.
- .env.example: variables demostrativas.
- README.md: documentacion del proyecto.

## Requisitos

- Docker Desktop funcionando.
- Puerto 8080 disponible.
- Navegador web.

## Construccion

docker build -t reserva-medica:1.0 .

## Ejecucion

docker compose up -d --build

## Verificacion

Abrir http://localhost:8080

docker compose ps
docker compose logs
docker stats --no-stream

## Detencion

docker compose down

## Seguridad

La aplicacion no utiliza credenciales reales
ni almacena informacion personal o clinica.
El formulario es exclusivamente demostrativo.

## Autor

Miguel Fajardo Toro
Ingenieria en Informatica - IACC
2026
