**Instalación de Docker**

![](Aspose.Words.7d9f361c-8750-4794-9d5b-5b5667431791.001.png)

**Índice**

- Preparación del entorno de trabajo
- Trabajar con imágenes de Docker
- Administrar contenedores de Docker

**Preparación del entorno de trabajo**

- Como siempre, primero debemos de actualizar nuestra máquina para empezar con la instalación![](Aspose.Words.7d9f361c-8750-4794-9d5b-5b5667431791.002.jpeg)
- A continuación, es necesario instalar unas cuantas dependencias necesarias para la instalación de docker
  - sudo apt install apt-transport-https ca-certificates curl software-properties-common
- También debemos de añadir la clave GPG para el repositorio oficial de Docker![](Aspose.Words.7d9f361c-8750-4794-9d5b-5b5667431791.003.jpeg)
- Agregamos el repositorio de Docker al sistema y actualizamos la máquina![](Aspose.Words.7d9f361c-8750-4794-9d5b-5b5667431791.004.jpeg)
- Ahora procedemos a instalar docker![](Aspose.Words.7d9f361c-8750-4794-9d5b-5b5667431791.005.jpeg)
- Comprobamos que el servicio se haya desplegado de manera correcta![](Aspose.Words.7d9f361c-8750-4794-9d5b-5b5667431791.006.jpeg)

**Trabajar con imágenes de docker**

- Ahora para probar docker, solo resta desplegar el siguiente comando
  - docker run hello-world
- Y así habremos desplegado nuestra primera aplicación con docker

**Administrar contenedores de docker**

- Con los comandos ps, ps-a y ps -l, veremos, en el mismo orden, los contenedores activos, activos e inactivos, y el último contenedor creado![](Aspose.Words.7d9f361c-8750-4794-9d5b-5b5667431791.007.jpeg)
- Y con docker images, se mostraran la nueva imagen, y la última de la que se derivó![](Aspose.Words.7d9f361c-8750-4794-9d5b-5b5667431791.008.jpeg)
Cristo Javier García Martín 2º DAW

DPL
