# Proyecto Docker

Proyecto académico utilizando Docker y contenedores conectados mediante una red interna.

## Contenedores utilizados
- MySQL
- Node.js
- Nginx

## Red Docker
app-network

## Objetivo
Implementar contenedores Docker comunicados entre sí mediante una red virtual.

## Comandos utilizados

docker network create app-network

## Creación de contenedores

docker run -d --name mysql-db --network app-network -e MYSQL_ROOT_PASSWORD=123456 mysql

docker run -dit --name nodeapp --network app-network node bash

docker run -d --name webserver --network app-network -p 80:80 nginx


## Validación de comunicación

Se verificó la comunicación entre los contenedores:

ping mysql-db
ping webserver

## Resultados

-Comunicación exitosa entre contenedores
-0% de pérdida de paquetes
-Correcta resolución de nombres dentro de la red Docker
-Disponibilidad de los servicios desplegados 

## Integración Continua con Jenkins

Como parte de la Entrega se implementó Jenkins utilizando Docker como plataforma de despliegue

## actividades realizadas 

-Instalación de Jenkins mediante Docker
-Configuración del usuario administrador
-Creación del proyecto Freestyle llamado proyecto8
-Integración con GitHub
-Configuración de tareas de construcción
-Ejecución de compilaciones automáticas

## Repositorio integrado

https://github.com/lrojano/proyecto8.git

## Resultado de Jenkins

Jenkins logró:

-Conectarse al repositorio GitHub
-Descargar automáticamente el código fuente
-Ejecutar tareas de construcción
-Mostrar registros de ejecución
-Finalizar exitosamente las compilaciones

Resultado final:

Finished: SUCCESS

## Implementación de Pipeline Jenkins

Como mejora al proceso de Integración Continua, se implementó un Pipeline Jenkins utilizando 
un archivo Jenkinsfile almacenado en el repositorio GitHub

El Pipeline ejecuta automáticamente las siguientes tareas:

- Verificación de la versión de Git
- Validación del contenido del repositorio
- Ejecución de etapas automatizadas de Integración Continua
- Generación de resultados en la consola de Jenkins

Resultado obtenido:

PIPELINE EJECUTADO CORRECTAMENTE
Finished: SUCCESS

## Evidencias

Las evidencias del proceso se encuentran en la carpeta:

Capturas de Pantalla/

Incluyen:

- Instalación de Docker
- Descarga de imágenes
- Creación de contenedores
- Configuración de red
- Validación de comunicación entre contenedores
- Instalación de Jenkins
- Configuración del proyecto Jenkins
- Integración con GitHub
- Compilaciones exitosas

## Tecnologías utilizadas

- Docker Desktop
- Jenkins
- Git
- GitHub
- MySQL
- Node.js
- Nginx

## Conclusiones

- Se implementó exitosamente una arquitectura basada en contenedores Docker
- Se verificó la comunicación entre servicios mediante redes virtuales
- Jenkins permitió automatizar actividades de Integración Continua
- La integración con GitHub facilitó la validación automática del repositorio
- El proyecto obtuvo compilaciones exitosas demostrando el correcto funcionamiento de la solución
- Se implementó un Pipeline Jenkins basado en un archivo Jenkinsfile almacenado en GitHub

## Imágenes del proyecto
  
### Visual
<img width="2711" height="1439" alt="image" src="https://github.com/user-attachments/assets/7b75ab20-fa76-4c64-b1ec-1a8433de483b" />

### MySQL
<img width="2649" height="1439" alt="image" src="https://github.com/user-attachments/assets/d1543fa8-15b5-4f69-9267-ee667a2511c3" />

### Terminal Git

<img width="1077" height="695" alt="image" src="https://github.com/user-attachments/assets/49b41345-b18a-449d-8dba-e30b27fe3f81" />

### Base Visualizada LocalHost 3000

<img width="1732" height="1439" alt="image" src="https://github.com/user-attachments/assets/ffaf1687-8270-4944-b395-fe6111207a01" />

### jenkins ejecutado proyecto8

<img width="1892" height="827" alt="Jenkins ejecutado proyecto8" src="https://github.com/user-attachments/assets/eca7fba6-6299-465c-ba04-a119651af6dd" />




 

