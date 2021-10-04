Instalación Git Lab

![](Aspose.Words.944b6acc-5c1e-4db9-b223-168d674e2fdb.001.png)

Índice

- Actualización de los repositorios
- Ejercicio Instalación de paquetes adicionales
- Instalación de Gitlab
- Acceso

Actualización de los repositorios

- Para comenzar con la práctica, debemos de actualizar tanto el repositorio como el sistema operativo que estemos usando. En el caso de linux, serían los siguientes comandos:![](Aspose.Words.944b6acc-5c1e-4db9-b223-168d674e2fdb.002.jpeg)
  - sudo apt update && sudo apt upgrade

Instalación de paquetes adicionales![](Aspose.Words.944b6acc-5c1e-4db9-b223-168d674e2fdb.003.jpeg)

- Ahora debemos de instalar unos paquetes adicionales necesarios para la instalación de Gitlab en sistemas Ubuntu:![](Aspose.Words.944b6acc-5c1e-4db9-b223-168d674e2fdb.004.jpeg)![](Aspose.Words.944b6acc-5c1e-4db9-b223-168d674e2fdb.005.jpeg)
  - sudo apt install -y vim curl ca-certificates apt-transport-https

Instalación de Gitlab

- La instalación la realizaremos mediante el propio script que nos proporciona el equipo de Gitlab. Ejecutaremos el siguiente comando
  - curl -s https://packages.gitlab.com/install/repositories/gitlab/gitlab-ce/sc ript.deb.sh | sudo bash
- Seguido de
  - sudo apt install gitlab-ce
- Para terminar con la instalación debemos de ejecutar el siguiente comando y habremos finalizado![](Aspose.Words.944b6acc-5c1e-4db9-b223-168d674e2fdb.006.jpeg)![](Aspose.Words.944b6acc-5c1e-4db9-b223-168d674e2fdb.007.jpeg)
  - sudo gitlab-ctl reconfigure
Cristo Javier García Martín 2º DAW

Despliegue de Aplicaciones Web
