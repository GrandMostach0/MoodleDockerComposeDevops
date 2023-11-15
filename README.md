## Ejercicio Examen, despliegue de una aplicacion con docker-compose ☝️

## *instalación moodle utilizando el docker-compose para levantar los servicios de moodle, y mariadb, teniendo como fin una creación de un curso con participantes y deferentes roles*

 Clonar el repositorio de GitHub donde estará en la documentación para la instalación, repositorio de GitHub(GrandMostach0): 
 ```console
https://github.com/GrandMostach0/MoodleDockerComposeDevops.git
```
una vez clonado el repositorio procedemos cambiarnos de directorio con el comando:
```console
    cd MoodelDockerComposeDevops 
   ```
   Una vez ya estando en el directorio procedemos a realizar los siguientes comandos:

 1. utilizar el comando docker-compose de la imagen **bitnami/moodle** para levantar el docker-compose de esa imagen, el código es: 
 ```console
curl -sSL https://raw.githubusercontent.com/bitnami/containers/main/bitnami/moodle/docker-compose.yml > docker-compose.yml
docker-compose up -d
```
2. para ver si el contenedor está corriendo ejecutamos el código de Docker siguiente, donde también nos muestra que está corriendo en el puerto 80:
 ```console
docker ps 
```
##
## Demostración de que esta corriendo 
[Http://localhost:80/](http://localhost:80/)

## Configuración de la cuenta del administrador
ahora que vemos está funcionando le damos el botón de **login** que se encuentra en la parte izquierda superior.
Credenciales que tiene como default:
*username: user*
*Password: bitnami*


## demostración de que si se accedió al panel de administración
 [docker_4]
 ## Creación del curso
 para crear el curso tenemos que ir a:
 *Site administration ---> Courses ---> Add new Course*

Demostración que el curso se ha creado correctamente
[imagen]

## ahora configuramos el perfil del administrador

*haciendo click en nuestro perfil ---> edit profile*

[imagen de edición]

demostracion de los cambios guardados
[imagen demostracion]

##
## agregando mas personas al curso con sus roles
para agregar más personas tenemos que ir en: *site administration ---> users -->add new user*

## ahora vamos a agregar a las personas que agregamos recientemente 
en *curso1 ---> participants ---> Enrol users*
[imagen]

agregamos a lugo como estudiante
[imagen]

agregamos a raul como maestro
[imagen]

-----------------------------------
Ahora ya podemos ver a los participantes inscritos en el curso 1
[imagen]
