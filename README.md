# Dockerizacion de las Aplicaciones

[Naokipanel](https://github.com/naoki-solutions/naokipanel) tiene como objetivo facilitar la tarea de automatizar todos los servicios internos de la organizacion, esta herramienta consta de una pequeña aplicacion web donde se pueden administrar todos los contenedores de [Docker](https://docker.com) mediante un simple dashboard.

## Contenido

* Migracion de repositorios 
* Dockerizacion de las aplicaciones
* Despliegue en produccion (Proximamente)

### Migracion de repositorios 

**En primer lugar, todos los repositorios con proyectos de la organizacion deberan ser transferidos a nuevos repositorios alojados aqui.**

1) Transfiere tu repositorio yendo a la configuracion de tu repo y ve al apartado de Danger Zone - Transfer Ownership. 👇
![Section 1](/assets/img/section1-transfer.png)

2) Completa los campos, el nuevo owner del repositorio y typea el nombre de tu repo incluyendo el dominio, para confirmar. 👇
![Section 2](/assets/img/section2-transfer.png)

### Dockerizacion de las aplicaciones

En esta etapa se debera configurar un par de scripts con el objetivo construir una imagen de su proyecto y sus dependencias para luego ser utilizada por un contenedor en nuestra infraestructura.

1) Copiar los archivos necesarios que correspondan a tu lenguaje y pegalos en el directorio raiz de ru proyecto.

[**Archivos de docker**](https://github.com/naoki-solutions/Services-Demo-Template)

2) Luego deberas modificar los campos de forma que corresponda a tu aplicacion.

**ACLARACION:** Si utizas python o javascript los archivos prefabricados de docker son compatibles con la mayoria de los stacks de los proyectos que se realizan aqui.

### Despliegue de la aplicacion

**ATENCION:** Debido a que ahun estamos en desarrollo, esta seccion se mantendra en blanco hasta que se termine con el desarrollo de la aplicacion Naokipanel.
