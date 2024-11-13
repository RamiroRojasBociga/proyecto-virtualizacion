# Proyecto de Virtualización

Este proyecto tiene como objetivo crear una solución de virtualización para una organización.
La organización quiere consolidar su infraestructura, que actualmente está distribuida en tres servidores tipo torre. Se ha adquirido un nuevo servidor más potente, y el objetivo es crear tres contenedores en él que proporcionen los siguientes servicios:

- Apache
- MySQL
- Nginx

Además, se debe configurar RAID LV1 para los tres servicios y utilizar Podman para replicar las imágenes Docker. El trabajo se documentará paso a paso en esta bitácora.

## Bitácora

### Fecha: 12 de noviembre de 2024
- **Inicio del proyecto:** Se ha creado el repositorio en GitHub y se ha configurado el archivo `README.md` para la documentación.


- **Imagen modificacion archivo README**
![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20del%20README.png?raw=true)

- **Discos que se van a utilizar para la creacion de los Raid nivel 1**
- ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Discos%20para%20raid.png)

