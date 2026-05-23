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

docker run -d --name mysql-db --network app-network -e MYSQL_ROOT_PASSWORD=123456 mysql

docker run -dit --name nodeapp --network app-network node bash

docker run -d --name webserver --network app-network -p 80:80 nginx


## Validación de comunicación

Se verificó la comunicación entre los contenedores:

ping mysql-db
ping webserver

## Resultados

- Comunicación exitosa 
- 0% pérdida de paquetes 


## Evidencias

Las evidencias del proceso se encuentran en la carpeta:

Capturas de Pantalla/

Incluyen:

- Instalación de Docker
- Descarga de imágenes
- Creación de contenedores
- Configuración de red
- Validación de comunicación entre contenedores
