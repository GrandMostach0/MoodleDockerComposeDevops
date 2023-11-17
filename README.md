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

1. para correr el contenedor
```console
    sudo docker compose up
   ```
*(si deseamos que sea en segundo plano solo agregamo al final un -d)*

2. para detener el contenedor si estamos en segundo plano
```console
    docker compose down
   ```
*(si no estamos en segundo plano entonces utilizamos (ctrl + c) y debe funcionar)*

##
## Demostración de que esta corriendo 
[Http://localhost:80/](http://localhost:80/)

![dockerCompose_3](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/354d78fa-b5b3-46ec-9eae-774b5492051f)


## Configuración de la cuenta del administrador
ahora que vemos está funcionando le damos el botón de **login** que se encuentra en la parte izquierda superior.
Credenciales que tiene como default:
*username: user*
*Password: bitnami*

![dockerCompose_4](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/4f85e6f2-ee37-437a-9653-b20f1c20331b)

 ## Creación del curso
 para crear el curso tenemos que ir a:
 *Site administration ---> Courses ---> Add new Course*
![dockerCompose_5](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/2c10a1c9-51cb-41b5-9bbb-dcffdbbbade3)

Demostración que el curso se ha creado correctamente

![dockerCompose_6](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/2a7a2b37-86a3-4e5c-a96f-39f597998bba)

## ahora configuramos el perfil del administrador
*haciendo click en nuestro perfil ---> edit profile*
![dockerCompose_7](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/389a9882-6981-463a-bc12-c74d6dad7c60)

demostracion de los cambios guardados
![dockerCompose_9](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/dbbd9360-fd80-46b9-8279-329a5827e9f6)

##
## agregando mas personas al curso con sus roles
para agregar más personas tenemos que ir en: *site administration ---> users -->add new user*
![dockerCompose_10](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/d875a211-882a-43ae-b34b-fb4f0dd1e1b1)

## ahora vamos a agregar a las personas que agregamos recientemente 
en *curso1 ---> participants ---> Enrol users*
![dockerCompose_11](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/e3aea5e8-3034-4f2e-a6d6-82c17caf8c51)


agregamos a lugo como estudiante

![dockerCompose_12](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/57d076b2-9c12-4368-a21a-0e9973878ac5)

agregamos a raul como maestro

![dockerCompose_13](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/277c24a0-57f7-400e-890a-70a5c6cb75ca)

-----------------------------------
Ahora ya podemos ver a los participantes inscritos en el curso 1
![dockerCompose_14](https://github.com/GrandMostach0/MoodleDockerComposeDevops/assets/75960744/2f3e78de-baf1-477b-bb26-d1ea76c14e6f)

