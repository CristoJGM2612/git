Instalación de Apache Tomcat

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.001.png)

Índice

- Requisitos Previos
- Instalación en local

Requisitos Previos

- Antes de empezar con la instalación, es necesario tener instalado java, lo haremos con el siguiente comando:
  - sudo apt install default-jdk

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.002.png)

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.003.png)

Instalación en local

- Luego de comprobar que disponemos de java, debemos de descargar el paquete desde la página oficial de apache
  - wget https://downloads.apache.org/tomcat/tomcat-10/v10.0.16/bin/ apache-tomcat-10.0.16.tar.gz

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.004.png)

- Seguidamente, debemos de añadir nuestro usuario tomcat:
  - sudo useradd -U -m -d /opt/tomcat -k /dev/null -s /bin/false tomcat

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.005.png)

- Y descomprimimos el archivo en su localización definitiva

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.006.png)

- Ahora debemos de asignar como propietario de la carpeta, al usuario antes creado, y configuramos nuestro servicio tomat

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.007.png)

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.008.jpeg)

- Podemos comprobar si hemos realizado el servicio de manera adecuada con los siguientes comandos:
  - sudo systemctl start tomcat10
  - sudo systemctl status tomcat10

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.009.png)

- Cabe añadir, que he modificado el puerto de despliegue en el archivo server.xml

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.010.png)

![](Aspose.Words.942763fb-a2d7-47c1-aa7b-8562071203b1.011.jpeg)
Cristo Javier García Martín 2º DAW

DPL
