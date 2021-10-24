**JBoss-Wildfly**

![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.001.png)

**Índice**

- Requisitos previos
- Instalación de Wildfly en local
- Cómo añadir usuarios a Wildfly

**Requisitos Previos**

- Necesitarás un sistema Linux
- Java
- Maven

**Pasos para realizar la instalación en local**

- Primero, debemos de actualizar los repositorios de nuestro sistema![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.002.jpeg)
- A continuación, debemos de descargar nuestro paquete de WildFly
- Ahora crearemos el nuevo grupo y usuario wildfly:![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.003.jpeg)![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.004.jpeg)
- Descomprimimos el recién descargado paquete de Wildly y movemos a la carpeta de destino, en este caso /opt/wildfly![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.005.jpeg)![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.006.jpeg)
- Y creamos un enlace simbólico con el siguiente comando
- sudo ln -s /opt/wildfly-25.0.0.Final /opt/wildfly
- Además, otorgamos acceso al usuario y grupo wildfly![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.007.jpeg)
- Seguidamente, configuraremos el inicio del servidor con los siguientes comandos
- sudo mkdir -p /etc/wildfly
- sudo cp /opt/wildfly/docs/contrib/scripts/systemd/wildfly.conf /etc/wildfly/
- Procederemos con los siguientes comandos para terminar de configurar el arranque del servidor
- sudo cp /opt/wildfly/docs/contrib/scripts/systemd/launch.sh /opt/wildfly/bin/
- sudo sh -c 'chmod +x /opt/wildfly/bin/\*.sh'
- sudo cp /opt/wildfly/docs/contrib/scripts/systemd/wildfly.service /etc/systemd/system/
- sudo systemctl daemon-reload![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.008.jpeg)
- sudo systemctl restart wildfly.service
- Para terminar de configurar Wildfly, debemos de modificar el fichero de configuración y cambiar![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.009.jpeg) el rooteado de puertos al 8084:

**Cómo añadir usuario a Wildfly**

- Y para terminar, debemos de ejecutar el siguiente script![](Aspose.Words.21d90ee9-5928-4fb1-87a4-d6c10e57b4f0.010.jpeg)
- sudo /opt/wildfly/bin/add-user.sh
Cristo Javier García Martín 2º DAW

DPL
