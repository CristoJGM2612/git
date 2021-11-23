Despliegue de Servidor con balanceo de carga y 4 nodos +

![](Aspose.Words.a9a3a185-0b6f-4a75-8934-cfb7a5b0a23c.001.jpeg)

Índice

- Activación de módulos necesarios en Apache
- Configuración de Apache

Activación de los módulos necesarios en Apache

- Para comenzar, debemos de activar los siguientes módulos en Apache:![](Aspose.Words.a9a3a185-0b6f-4a75-8934-cfb7a5b0a23c.002.jpeg)

a2enmod proxy

a2enmod proxy\_http

a2enmod proxy\_ajp

a2enmod rewrite

a2enmod deflate

a2enmod headers

a2enmod proxy\_balancer a2enmod proxy\_connect a2enmod proxy\_html

a2enmod lbmethod\_byrequests

Configuración de Apache

- Seguidamente debemos de configurar apache y añadir las siguientes líneas:

![](Aspose.Words.a9a3a185-0b6f-4a75-8934-cfb7a5b0a23c.003.png)

**Preparación del Proyecto![](Aspose.Words.a9a3a185-0b6f-4a75-8934-cfb7a5b0a23c.004.jpeg)**

- Nos descargamos el repositorio de la asignatura e instalamos las dependecias con
  - mvn clean install

**Configuración de Dockerfile y docker-compose.yml![](Aspose.Words.a9a3a185-0b6f-4a75-8934-cfb7a5b0a23c.005.jpeg)**

- Ahora debemos de configurar de la siguiente forma tanto el Dockerfile, como el docker-compose.yml
- Dockerfile
- docker-compose.yml![](Aspose.Words.a9a3a185-0b6f-4a75-8934-cfb7a5b0a23c.006.jpeg)
- Levantamos el servicio con sudo docker-compose up -d, y revisamos la siguiente dirección![](Aspose.Words.a9a3a185-0b6f-4a75-8934-cfb7a5b0a23c.007.jpeg)

localhost/app-web-demo![](Aspose.Words.a9a3a185-0b6f-4a75-8934-cfb7a5b0a23c.008.jpeg)![](Aspose.Words.a9a3a185-0b6f-4a75-8934-cfb7a5b0a23c.009.jpeg)
Cristo Javier García Martín 2º DAW

DPL
