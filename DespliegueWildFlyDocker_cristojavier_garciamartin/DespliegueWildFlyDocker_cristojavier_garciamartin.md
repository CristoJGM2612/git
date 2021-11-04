Despliegue WildFly en Docker

Índice

- Descarga de la imagen del docker WildFly
- Comprobación del servicio

Descarga de la imagen de docker WildFly![](Aspose.Words.8db358ce-5c30-48d6-ac6a-a3aaf33eedac.001.jpeg)

- Primero debemos de descargar nuestra imagen docker de WildFly
- Seguidamente verificamos las imágenes descargadas en nuestro sistema![](Aspose.Words.8db358ce-5c30-48d6-ac6a-a3aaf33eedac.002.jpeg)![](Aspose.Words.8db358ce-5c30-48d6-ac6a-a3aaf33eedac.003.jpeg)
- Ahora procedemos a arrancar nuestro contenedor de Wildfly con el siguiente comando:

sudo docker run -d -p 5000:8080 --name "servidor-desa" jboss/wildfly

- Donde:
  - -d arranca el servidor en el background
  - -p 5000:8080 especifica el puerto 8080 y el host 5000 (nuestra máquina)![](Aspose.Words.8db358ce-5c30-48d6-ac6a-a3aaf33eedac.004.jpeg)
  - --name “servidor-desa” Define el alias para nuestro contenedor

**Comprobación del servicio**

- A continuación verificamos la ip asignada a docker y verificamos que nuestro servidor se haya desplegado![](Aspose.Words.8db358ce-5c30-48d6-ac6a-a3aaf33eedac.004.jpeg)![](Aspose.Words.8db358ce-5c30-48d6-ac6a-a3aaf33eedac.005.jpeg)
