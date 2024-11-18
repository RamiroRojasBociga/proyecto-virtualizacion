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


### Fecha: 12 de noviembre de 2024
- **Discos que se van a utilizar para la creacion de los Raid nivel 1**
- ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Discos%20para%20raid.png)

- **Creacion de Raid nivel 1**
- ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/7360178289677da1d0b4f135909b04ff9db93321/Creacion%20de%20raid.png)

- **Creacion de volumenes fisicos**
-  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20volumenes%20fisicos.png?raw=true)

- **Creacion de grupo de volumenes**
-  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20grupo%20de%20volumenes.png?raw=true)

- **Creacion de volumenes logicos**
-  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20Volumenes%20Logicos.png?raw=true)

-  
