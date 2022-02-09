# Bsale Challenge


Objetivo del proyecto: Crear una tienda online completa(front y backend) con la finalidad de mostrar productos basado en busqueda y filtros.

Las Caractericas de la aplicacion: 
* Frontend simple que despliega productos por busqueda dinamicamente
* Backedn(Api rest) que proporciona endpoinds necesarios por la aplicacion

## Tecnologias y Librerias usadas
Frontend :
* Vanilla js
* Html
* Css
* Jquery
* Axios

Backend:
* Node.js
* Express
* Sequelize
* Cors
* Mysql2
* Dotenv

## Ejecucion

En este caso Se esta manejando dos entornos diferentes para el front y backend:

Fronend: En El front es simple y directo , No se esta manejando ningun framework para el fron asi que no hay requisitos para ejecutar
Unicamente debes apuntar correctamente al index.html en el entorno que estes ejecutando

```
$ ./console.py
(hbnb) help

Documented commands (type help <topic>):
========================================
EOF  help  quit

(hbnb) 
(hbnb) 
(hbnb) quit
$
```
Backend: En el caso del backedn es diferente, estamos usando el entorno de node.js, su manejador de 
paquetes es estupendo asi que la instalacion de las dependencias no deberia ser un problema.

Aqui tienes dos opciones:


* Para desarrollo: Estoy proporcionando los node-modules para facilitar las cosas , en caso de que quieras instalar las dependencias desde 0, 
ejecuta `npm install` y por ultimo `npm run dev`

```
(base) root@DESKTOP-VQ684KQ:/home/bsale-challenge/api# pwd
/home/bsale-challenge/api
(base) root@DESKTOP-VQ684KQ:/home/bsale-challenge/api# 
(base) root@DESKTOP-VQ684KQ:/home/bsale-challenge/api# npm install
...
...
...
(base) root@DESKTOP-VQ684KQ:/home/bsale-challenge/api# npm run dev

> api@1.0.0 dev
> nodemon ./src/index.js

[nodemon] 2.0.15
[nodemon] to restart at any time, enter `rs`
[nodemon] watching path(s): *.*
[nodemon] watching extensions: js,mjs,json
[nodemon] starting `node ./src/index.js`
Server is running on port 3000
Executing (default): SELECT 1+1 AS result
```
* Para produccion : Para produccion instalas las dependencias `npm install` seguido de `npm run start`
```
(base) root@DESKTOP-VQ684KQ:/home/bsale-challenge/api# pwd
/home/bsale-challenge/api
(base) root@DESKTOP-VQ684KQ:/home/bsale-challenge/api# 
(base) root@DESKTOP-VQ684KQ:/home/bsale-challenge/api# npm install
...
...
...
(base) root@DESKTOP-VQ684KQ:/home/bsale-challenge/api# npm run start

> api@1.0.0 start
> node ./src/index.js

Server is running on port 3000
Executing (default): SELECT 1+1 AS result
Connection has been established successfully.

```


## Estructura de archivos

##|Directorio o Archivo | Descripcion
---|---|---
0|[api](./api)| Directorio que contiene la logica de backend(api Rest)
1|[front](./front)| Directorio que contiene la logica de frontend


### Structura directorio API

##|Directorio o Archivo | Descripcion
---|---|---
0|[fakeData](./api/fakeData)| Contiene Data de Backup en caso de necesitarla en desarrollo
1|[node_modules](./api/node_modules)| Contiene todos las dependencias , en caso de necesitarla
2|[src](./api/src)| Directorio que contiene la logica de nuestra api 

### Structura directorio SRC

##|Directorio o Archivo | Descripcion
---|---|---
0|[models](./api/src/models)| Este directorio Contiene los modelos de nuestra db
1|[routes](./api/src/routes)| Este directorio Contiene todos los endpoints de nuestra aplicacion
2|[utils](./api/src/utils)| Este directorio Contiene funciones de utilidad 


### Structura directorio Front

##|Directorio o Archivo | Descripcion
---|---|---
0|[apicalls](./front/fakeData)| Este Directorio Contiene toda la logica de los apicalls a nuestra api
1|[galery](./front/node_modules)| Este Directorio contiene imagenes que usa nuestra app
2|[js](./api/src)| En este Directorio tenemos funciones de utilidad 
3|[pages](./api/src)| En este Directorio tenemos todas nuestas paginas html 
4|[styles](./api/src)| Este Directorio contiene todo nuestros archivos css



