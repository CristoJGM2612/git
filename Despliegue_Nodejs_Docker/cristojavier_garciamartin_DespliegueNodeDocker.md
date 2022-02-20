Desplegar una aplicación en Node.js en Docker

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.001.png)

Índice

- Preparación del entorno
- Creación de Node.js
- Creación de ficheros de Docker
- Construcción y despliegue de la imagen

Preparación del entorno

- Primero debemos de actualizar la máquina, y comprobar que tenemos node instalado

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.002.jpeg)

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.003.png)

Creación de Node.js

- Contenido del fichero package.json

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.004.jpeg)

- Contenido server.js

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.005.png)

Creación de ficheros de docker

- Contenido Dockerfile

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.006.jpeg)

- Contenido .dockerignore

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.007.png)

Construcción y despliegue de la imagen

- Construimos la imagen con el siguiente comando:
  - sudo docker build . -t cj/node-web-app

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.008.png)

- Y desplegamos la imagen con el siguiente comando:
  - sudo docker run -p 49160:8080 -d cj/node-web-app

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.009.png)

- Para finalizar, podemos probar la aplicación accediendo a localhost:49160:

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.010.png)

![](Aspose.Words.81b3d951-7797-4134-b10c-459165d4d5fc.011.png)
Cristo Javier García Martín 2º DAW

DPL
