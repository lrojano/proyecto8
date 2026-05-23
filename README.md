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

## Imágenes del proyecto
  
### Visual
<img width="2711" height="1439" alt="image" src="https://github.com/user-attachments/assets/7b75ab20-fa76-4c64-b1ec-1a8433de483b" />

### MySQL
<img width="2649" height="1439" alt="image" src="https://github.com/user-attachments/assets/d1543fa8-15b5-4f69-9267-ee667a2511c3" />

### Terminal Git

<img width="1077" height="695" alt="image" src="https://github.com/user-attachments/assets/49b41345-b18a-449d-8dba-e30b27fe3f81" />

### Base Visualizada LocalHost 3000

<img width="1732" height="1439" alt="image" src="https://github.com/user-attachments/assets/ffaf1687-8270-4944-b395-fe6111207a01" />

 

