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



- **Discos que se van a utilizar para la creacion de los Raid nivel 1**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Discos%20para%20raid.png)

- **Creacion de Raid nivel 1**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/7360178289677da1d0b4f135909b04ff9db93321/Creacion%20de%20raid.png)

- **Creacion de volumenes fisicos**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20volumenes%20fisicos.png?raw=true)

- **Creacion de grupo de volumenes**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20grupo%20de%20volumenes.png?raw=true)

- **Creacion de volumenes logicos**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20Volumenes%20Logicos.png?raw=true)

- **Formatear Volumenes**
  
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Formatear%20los%20volumenes.png?raw=true)

- **Crear directorios para montaje**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Crear%20Directorios%20para%20montaje.png?raw=true)

- **Obtener UUID**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Obtener%20UUID.png?raw=true)

- **Modificacion archivo fstab**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Modificacion%20archivo%20fstab.png?raw=true)

- **Creacion de directorio para Apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/40870a554c0b690856979732c246f12bbf55d181/Creacion%20directorio%20para%20apache.png)

- **Creacion de archivo dockerfile para Apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/c11e82689b4335badcb1a5fc9a916d9fecb82d54/Creacion%20archivo%20Dockerfile.png)

- **Contenido del archivo dockerfile para Apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/546d2acae52a855c7cf202c210131c53a8005389/Contenido%20Archivo%20dockerfile.png)

- **Creacion directorio public-html para apache**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20directorio%20public-html.png?raw=true)

- **Creacion archivo index.html para apache**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Creacion%20archivo%20index%20html.png?raw=true)

- **Contenido archivo index.html para apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/c66d96ed61d0187ac84271355ed69262c9e28c54/Contenido%20Archivo%20index%20html.png)

- **Construir imagen de docker ara apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/49fabe3e5e35045894b37253199be30d94d48974/Construir%20imagen%20de%20docker.png)

- **Correr contenedor con la imagen de apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/7c5bf03b0732d52a248e84dad9567f1cfb64961b/Correr%20contenedor%20imagen%20de%20Apache.png)

- **Verificar contenedor corriendo apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/7c5bf03b0732d52a248e84dad9567f1cfb64961b/Correr%20contenedor%20imagen%20de%20Apache.png)

- **Verificacion del contenedor corriendo apache**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/8158c1d34dd5ba3380efaea07d593df3592231fe/Verificacion%20de%20contenedor%20corriendo%202.png)

- **Crear directorio para servidor mysql**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/1179e99f26bdd2aea78caed33686c5a13d6781d2/Crear%20directorio%20para%20servidor%20MySql.png)

- **Crear archivo dockerfile para mysql**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Crear%20archivo%20dockerfile%20para%20mysql.png?raw=true)

- **Editar archivo dockerfile para mysql**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Editar%20archivo%20dockerfile%20para%20mysql.png?raw=true)

- **Construir imagen de docker para mysql**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Construir%20imagen%20de%20docker%20para%20mysql.png?raw=true)

- **Crear y ejecutar contenedor para mysql**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Crear%20y%20ejecutar%20contenedor%20para%20mysql.png?raw=true)

- **Acceder a la consola de mysql**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Acceder%20a%20la%20consola%20de%20mysql.png?raw=true)

- **Acceder a mysql para cambios**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Acceder%20a%20mysql%20para%20cambios.png)

- **Insertar datos a la tabla**
  ![Descripción de la imagen](https://github.com/user-attachments/assets/3cad430f-3daf-4f21-891b-d8244f0f8c12)

- **Crear tabla empleados**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Crear%20tabla%20empleados.png)

- **Usar la tabla creada**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Usar%20la%20tabla%20creada.png?raw=true)

- **Crear base de datos sql**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Crear%20base%20de%20datos%20sql.png?raw=true)

- **Ingresar al contenedor de mysql**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/52f3fe0a48446ed210d94b18bfc1e916b0a8f535/Ingresar%20al%20contenedor%20de%20mysql.png)

- **Ejecutar el contenedor nginx**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/fd4875277a9079f006f4c3d3c0bc75ae95ca9acd/Ejecutar%20el%20contenedor%20nginx.png)

- **Crear y ejecutar contenedor nginx**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Crear%20y%20ejecutar%20contenedor%20nginx.png)

- **Construir imagen nginx**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/commit/9cb9deb43ce902b6f6334b20a112a16b8913b2a7)

- **Creacion archivo index nginx**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/ece8bb5f1e779d973be0e55c26000fea66f8720c/Creacion%20archivo%20index%20nginx.png)

- **Crear directorio para nginx**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/8aa3d996645ce8931cb853372f82ed8be0d35140/Crear%20directorio%20para%20nginx.png)

- **Editar archivo index nginx**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Editar%20archivo%20index%20nginx.png)

- **Crear directorio para archivos web nginx**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Crear%20directorio%20para%20archivos%20web.png?raw=true)

- **Creacion archivo Dockerfile nginx**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/d171db386a9713458cf00f40cbd4bd55b09bbc2f/Creacion%20archivo%20Dockerfile%20nginx.png)

- **Editar archivo dockerfile para nginx**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Editar%20archivo%20dockerfile%20para%20nginx.png?raw=true)

- **Prueba del servicio nginx**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Prueba%20del%20servicio%20nginx.png?raw=true)

- **Cambios en nginx**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Cambios%20en%20nginx.png?raw=true)

- **Crear directorio apache podman**
  ![Descripción de la imagen](https://github.com/RamiroRojasBociga/proyecto-virtualizacion/blob/main/Crear%20directorio%20apache%20podman.png?raw=true)

- **Creacion archivo Dockerfile apache podman**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/57ba61333813127a007bf232512ee385aff31e1c/Creacion%20archivo%20Dockerfile%20apache%20podman.png)

- **Editar archivo Dockerfile apache podman**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/ca45d0872c055fd7d416b3f393a679609691b6df/Editar%20archivo%20Dockerfile%20apache%20podman.png)

- **Construir imagen apache podman**
  ![Descripción de la imagen](https://raw.githubusercontent.com/RamiroRojasBociga/proyecto-virtualizacion/5d5e404f617ef28e15e9ae8d58792f3958e7fba6/Construir%20imagen%20apache%20podman.png)





