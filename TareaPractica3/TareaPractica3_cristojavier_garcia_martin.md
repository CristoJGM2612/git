Instalación Apache en linux

![](Aspose.Words.a66b2535-0119-4d69-9daa-6a983a563915.001.jpeg)

Índice

- Actualización de los repositorios
- Instalación de Apache
- Acceso

Actualización de los repositorios

- Para comenzar con la práctica, debemos de actualizar tanto el repositorio como el sistema operativo que estemos usando. En el caso de linux, serían los siguientes comandos:![](Aspose.Words.a66b2535-0119-4d69-9daa-6a983a563915.002.jpeg)
  - sudo apt update && sudo apt upgrade

Instalación de Apache![](Aspose.Words.a66b2535-0119-4d69-9daa-6a983a563915.003.jpeg)

- A continuación instalaremos apache teniendo en cuenta que dará error, pues ya tenemos Gitlab instalado y, de forma nativa, ambos usan el mismo puerto, por lo que tendremos que configurar los puertos de apache. Yo utilicé el 8081, en vez del 80 que viene por defecto y es el nativo tanto de Apache como Gitlab![](Aspose.Words.a66b2535-0119-4d69-9daa-6a983a563915.004.jpeg)![](Aspose.Words.a66b2535-0119-4d69-9daa-6a983a563915.005.jpeg)
  - sudo apt install apache2

Acceso

- Luego de configurar los puertos, reiniciamos apache y revisamos la configuración de firewall con los siguientes comandos![](Aspose.Words.a66b2535-0119-4d69-9daa-6a983a563915.006.jpeg)![](Aspose.Words.a66b2535-0119-4d69-9daa-6a983a563915.007.jpeg)
  - sudo systemctl restart apache2
  - sudo ufw app list
Cristo Javier García Martín 2º DAW

Despliegue de aplicaciones Web
