**Instalación de PHP en Nginx**

![](Aspose.Words.c7641760-4590-471c-bdc4-e916e4cfdc1e.001.png)

**Índice**

- Actualización de repositorios
- Instalación y configuración de PHP
- Comprobación de correcta instalación

**Actualización de repositorios![](Aspose.Words.c7641760-4590-471c-bdc4-e916e4cfdc1e.002.jpeg)**

- Para comenzar, actualizaremos nuestra máquina como ya es costumbre

**Instalación y configuración de PHP![](Aspose.Words.c7641760-4590-471c-bdc4-e916e4cfdc1e.003.jpeg)**

- A continuación, procederemos a instalar el paquete de PHP que necesitamos al usar nginx
- Seguidamente debemos de modificar el fichero situado en la carpeta![](Aspose.Words.c7641760-4590-471c-bdc4-e916e4cfdc1e.004.jpeg)
  - /etc/nginx/sites-available/default

**Comprobación de configuración**

- Ahora solo resta crear un fichero php con la siguiente línea <?php phpinfo(): ?>, en la carpeta /var/www/html/![](Aspose.Words.c7641760-4590-471c-bdc4-e916e4cfdc1e.005.jpeg)
Cristo Javier García Martín 2º DAW

DPL
