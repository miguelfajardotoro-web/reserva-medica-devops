
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


## Pruebas y criterios de aceptacion

Para validar el funcionamiento del proyecto se
establecieron los siguientes criterios:

1. Construir la imagen Docker reserva-medica:1.0.
2. Ejecutar el servicio mediante Docker Compose.
3. Acceder a la aplicacion en http://localhost:8080.
4. Verificar el formulario de reserva de horas medicas.
5. Seleccionar especialidad, profesional, fecha y horario.
6. Comprobar la respuesta HTTP 200 de Nginx.
7. Verificar la carga correcta del archivo styles.css.
8. Revisar los registros del contenedor Docker.
9. Confirmar que no se almacenan datos personales reales.

## Resultados de las pruebas locales

Durante las pruebas realizadas se obtuvo:

- Construccion exitosa de la imagen Docker.
- Ejecucion del servicio mediante Docker Compose.
- Respuesta HTTP 200 para la pagina principal.
- Respuesta HTTP 200 para el archivo styles.css.
- Visualizacion correcta del formulario medico.
- Seleccion correcta de los campos demostrativos.
- Inicializacion correcta del servidor Nginx.

Las pruebas respaldan la preparacion de la version
inicial v1.0.0 del proyecto DevOps IACC.
