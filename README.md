# [Primer meetup Grails en México!] (http://www.meetup.com/Mexico-City-Grails-Meetup/)
![alt text](https://worldvectorlogo.com/logos/grails.svg "Grails")

# Primera sesión
En la primera sesión haremos una sencilla aplicación con Grails para poder ver de manera practica cual es su funcionamiento.

# 1 Instalar SDK MAN
SDKMAN! es una herramienta para la gestión de versiones de múltiples kists de desarrollo de sofware en su mayoría de los que están basdos en Unix.
Lo usaremos para instalar Grails. Es una definición más simple si has usado node SDKMAN sería tú nvm o en el caso de python tú pip.
- Para la instalación sigue los siguientes pasos en tu terminal.
```
$ curl -s get.sdkman.io | bash
```
```
$ source "$HOME/.sdkman/bin/sdkman-init.sh"
```
Para probar que todo este bien, usar el siguiente comando, este nos debe arrojar la versión de el sdk instalado, si es así todo ha salido como lo esperamos.
En caso de que no, podemos consultar la página oficial de [SDKMAN.](http://sdkman.io/install.html)
```
$ sdk version
```
Una vez que hemos instalado sdkman descarguemos Grails!

# 2 Instalar Grails
Esto descargará la versión más actual y estable de Grails, si quieres descargar un versión en especifico es necesario ingresar la versión después de "grails"
```
$ sdk install grails
```

# 3 Crear mi primer aplicación Grails
Cuando estemos en la terminal teclear el siguiente comando para crear nuestra primer app.
```
$ grails create-app meetup
```
Entrar a la carpeta de tú proyecto.
```
$ cd meetup
```
Entrar a la terminal de grails.
```
$ grails
```
Crear un contrlador de prueba.
```
grails> create-controller test
```
Ahora entremos a nuestro proyecto y busquemos el controlador Test, este se encuentra dentro de la carpeta grails-app, dentro de controladores. Una vez que estemos ahí, modifiquemos el controlados y rendereemos un mensaje, este puede ser el que queramos, en mi caso puse esto :
```java
package meetup

class TestController {

    def index() { 
    	render ":D Hola, estoy probando Grails!"
    }
}
```
Lo siguiente que haremos será correr nuestra aplicación con el siguiente comando.
```
grails> run-app 
```
Y listo, pueden entrar a el navegador en http://localhost:8080, dar click al link que los lleva al controlador y si todo salió bien, podrán ver su mensaje.
Esto es una practica demasiado simple, como una introducción para explorar la estructura de el proyecto y las funciones simples, según se definamos intereses la siguiente practica haremos algo más útil.

# Dudas
Cualquier duda y/o sugerecia, por favor, no duden en preguntarme estoy en la mejor disposición de ayudarles, en la sección de contribuidores estan mis datos de contacto. También agradecería saber cuales son sus intereses y espectativas.


# Contributors
- Gloria Palma González / ing.gloriapalmagonzalez@gmail.com / @GloriaPalmaGlez