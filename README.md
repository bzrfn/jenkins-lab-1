# Jenkins — Lab 1

Práctica académica para desplegar Jenkins LTS con JDK 21 en Docker y ejecutar un primer Job de tipo Freestyle.

## Objetivo

Crear un entorno Jenkins persistente, completar la configuración inicial y comprobar la ejecución de un Job que imprime `Hola mundo` en la salida de consola.

## Requisitos

- Docker Engine o Docker Desktop en ejecución.
- Git.
- Navegador web.

## Procedimiento general

1. Crear el volumen administrado `jenkins_home`.
2. Ejecutar `jenkins/jenkins:lts-jdk21` en el puerto local 8081.
3. Abrir `http://127.0.0.1:8081`.
4. Desbloquear Jenkins sin guardar la contraseña inicial en el repositorio.
5. Instalar los plugins sugeridos y completar la configuración inicial.
6. Crear el Job Freestyle `pipe-hola-mundo`.
7. Agregar un paso **Execute shell** con `echo "Hola mundo"`.
8. Ejecutar el Build y comprobar `Finished: SUCCESS`.

Los comandos reproducibles se encuentran en `commands/jenkins-docker.txt` y el script del ejemplo en `scripts/hello-world.sh`.

## Seguridad

Este repositorio no contiene contraseñas, tokens, credenciales ni el directorio interno de Jenkins.
