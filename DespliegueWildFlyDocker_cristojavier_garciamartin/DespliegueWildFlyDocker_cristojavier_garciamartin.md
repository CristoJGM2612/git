Despliegue WildFly en Docker

![](Aspose.Words.2442ba50-5f29-4337-9968-2b0dd438c239.001.jpeg)

**Índice**

- Descarga de la imagen del docker WildFly
- Comprobación del servicio

**Descarga de la imagen de docker WildFly![](Aspose.Words.2442ba50-5f29-4337-9968-2b0dd438c239.002.jpeg)**

- Primero debemos de descargar nuestra imagen docker de WildFly
- Seguidamente verificamos las imágenes descargadas en nuestro sistema![](Aspose.Words.2442ba50-5f29-4337-9968-2b0dd438c239.003.jpeg)![](Aspose.Words.2442ba50-5f29-4337-9968-2b0dd438c239.004.jpeg)
- Ahora procedemos a arrancar nuestro contenedor de Wildfly con el siguiente comando:

sudo docker run -d -p 5000:8080 --name "servidor-desa" jboss/wildfly

- Donde:
  - -d arranca el servidor en el background
  - -p 5000:8080 especifica el puerto 8080 y el host 5000 (nuestra máquina)![](Aspose.Words.2442ba50-5f29-4337-9968-2b0dd438c239.005.jpeg)
  - --name “servidor-desa” Define el alias para nuestro contenedor

**Comprobación del servicio**

- A continuación verificamos la ip asignada a docker y verificamos que nuestro servidor se haya desplegado![](Aspose.Words.2442ba50-5f29-4337-9968-2b0dd438c239.005.jpeg)![](Aspose.Words.2442ba50-5f29-4337-9968-2b0dd438c239.006.jpeg)
Cristo Javier Garcia Martín 2º DAW

DPL
