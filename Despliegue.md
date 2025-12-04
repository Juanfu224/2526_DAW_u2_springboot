Para empezar a hacer esta practica, me he clonado el repositorio directamente desde el proyecto del profesor. Una vex descargado he generado la imagen con el siguiente comando:

```bash
docker build -t imagen-generada .
```

Una vez terminado de ejecutarse el comando aparecerá la imagen generada en nuestra lista de imagenes:
![alt text](image.png)

Para poder subirlo es necesario darle primero un tag y ya despues puede subirse a docker hub. Para poder hacerlo hay que ejecutar los siguiente comandos:

```bash
docker tag imagen-generada:latest juanfu224/imagen-generada:latest
```

Para poder comprobar que se ha subido correctamente y verlo en Docker Hub, puedes acceder al siguiente [enlace](https://hub.docker.com/r/juanfu224/imagen-generada)

Te tiene que aparecer el siguiente resultado![alt text](image-1.png)

Para hacerlo con el Git Actions he utilizado el del siguiente [enlace](https://github.com/marketplace/actions/build-and-push-docker-images#usage)

Para cambiar añádir mi nombre al lado del titulo de la pagina, he tenido que editar la siguiente linea en [build/resources/main/templates/index.html](build/resources/main/templates/index.html)

https://github.com/Juanfu224/2526_DAW_u2_springboot/blob/8fab9385dc4b327ad33474c0e3a9de5b99673d09/src/main/resources/templates/index.html#L11-L14

Al terminar lo he podido hacer todo, pero no he conseguido sacarlo con git actions, ya que no se como poner mi token de docker hub sin que esté hardcodeado. Esto es necesario para poder terminar de subirlo todo a mi docker hub
