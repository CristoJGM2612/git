Despliegue War en Apache Tomcat

![](Aspose.Words.333502fd-ccae-4626-a42c-635198924bde.001.png)

Índice

- Requisitos previos
- Modificación del proyecto en java
- Despliegue en tomcat

Requisitos Previos

- Previamente, debemos de tener instalado Maven en el equipo, con el siguiente comando:
  - sudo apt install maven

![](Aspose.Words.333502fd-ccae-4626-a42c-635198924bde.002.png)

Modificación del Proyecto en Java

- Debemos de modificar los siguientes archivos en el proyecto:
  - web.xml

![](Aspose.Words.333502fd-ccae-4626-a42c-635198924bde.003.png)

- index.jsp

![](Aspose.Words.333502fd-ccae-4626-a42c-635198924bde.004.png)

- pom.xml

![](Aspose.Words.333502fd-ccae-4626-a42c-635198924bde.005.jpeg)

Despliegue en Tomcat

- Para desplegar nuestra aplicación en tomcat, debemos de copiar el archivo .war en la carpeta webapps, además de configurar un usuario de tomcat:
  - Copiamos el archivo .war en webapps

![](Aspose.Words.333502fd-ccae-4626-a42c-635198924bde.006.png)

- Y para comprobar el despliegue de la aplicación, es tan sencillo como acceder a la siguiente url:
  - <http://localhost:8085/app-web-demo/>

![](Aspose.Words.333502fd-ccae-4626-a42c-635198924bde.007.png)
Cristo Javier García Martín 2º DAW

DPL
