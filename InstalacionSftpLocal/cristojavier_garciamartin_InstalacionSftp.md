Instalación Servidor SFTP

![](Aspose.Words.4a8afd4d-214e-4a9d-b8b2-49e95df6396d.001.jpeg)

Índice

- Instalación servidor SFTP
- Configuración Vsftpd.conf

Instalación servidor Sftp

- Primeramente, debemos de actualizar nuestra máquina.
  - sudo apt update && sudo apt upgrade

![](Aspose.Words.4a8afd4d-214e-4a9d-b8b2-49e95df6396d.002.png)

- Luego, instalamos el paquete vsftpd:
  - sudo apt install -y vsftpd

![](Aspose.Words.4a8afd4d-214e-4a9d-b8b2-49e95df6396d.003.png)

Configuración Vsftpd.conf

- Ahora, debemos de acceder al fichero de configuración de vsftpd.conf, situado en la carpeta /etc, y verificamos que tengamos las siguientes opciones habilitadas:
  - pasv\_enable=YES
  - pasv\_min\_port=30000
  - pasv\_max\_port=30050

![](Aspose.Words.4a8afd4d-214e-4a9d-b8b2-49e95df6396d.004.png)

- Recargamos el servidor, y lo probamos con el cliente filezilla:

![](Aspose.Words.4a8afd4d-214e-4a9d-b8b2-49e95df6396d.005.png)

- Accedemos al servidor con nuestro usuario y contraseña

![](Aspose.Words.4a8afd4d-214e-4a9d-b8b2-49e95df6396d.006.png)

![](Aspose.Words.4a8afd4d-214e-4a9d-b8b2-49e95df6396d.007.png)
Cristo Javier García Martín 2º DAW

DPL
