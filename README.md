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
-![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/dfe33930ee795caaf962020046cca7a8f589e0d0/Creacion%20archivo%20index%20html.png)


### Fecha: 12 de noviembre de 2024
- **Discos que se van a utilizar para la creacion de los Raid nivel 1**
-![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Discos%20para%20raid.png)

- **Creacion de Raid nivel 1**
-![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/7360178289677da1d0b4f135909b04ff9db93321/Creacion%20de%20raid.png)

- **Creacion de volumenes fisicos**
- ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20volumenes%20fisicos.png?raw=true)

- **Creacion de grupo de volumenes**
- ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20grupo%20de%20volumenes.png?raw=true)

- **Creacion de volumenes logicos**
- ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20Volumenes%20Logicos.png?raw=true)

- **Formatear Volumenes**
- ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Formatear%20los%20volumenes.png?raw=true)

-  **Crear directorios para montaje**
![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Crear%20Directorios%20para%20montaje.png?raw=true)

-  **Obtener UUID**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Obtener%20UUID.png?raw=true)

-  **Modificacion archivo fstab**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Modificacion%20archivo%20fstab.png?raw=true)

-  **Creacion de directorio para Apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/40870a554c0b690856979732c246f12bbf55d181/Creacion%20directorio%20para%20apache.png)

-  **Creacion de archivo dockerfile**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/c11e82689b4335badcb1a5fc9a916d9fecb82d54/Creacion%20archivo%20Dockerfile.png)

-  **Contenido del archivo dockerfile**
![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/546d2acae52a855c7cf202c210131c53a8005389/Contenido%20Archivo%20dockerfile.png)

- **Creacion directorio public-html**
![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20directorio%20public-html.png?raw=true)

- **Creacion archivo index.html**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20archivo%20index%20html.png?raw=true)

  - **Contenido archivo index.html**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/c66d96ed61d0187ac84271355ed69262c9e28c54/Contenido%20Archivo%20index%20html.png)

- **Construir imagen de docker**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/49fabe3e5e35045894b37253199be30d94d48974/Construir%20imagen%20de%20docker.png)

- **Correr contenedor con la imagen de apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/7c5bf03b0732d52a248e84dad9567f1cfb64961b/Correr%20contenedor%20imagen%20de%20Apache.png)

- **Verificacion del contenedor corriendo**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/1fc927c19a94a2edeab807bbd78e4af714ec2e62/Verificacion%20de%20contenedor%20corriendo.png)
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/8158c1d34dd5ba3380efaea07d593df3592231fe/Verificacion%20de%20contenedor%20corriendo%202.png)






