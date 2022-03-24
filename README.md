# Xdebug-en-VSCODE
Guía de instalación de Xdebug en VSCODE


![](assets/README-dd1cb4e1.png)


# Índice #
<hr/>

- ## Software de esta instalación ##

- ## VS Code - PHP Debug ##

- ## Xdebug ##

- ## VS Code - launch.json ##

- ## Xdebug en acción ##

<hr/>

**Software de esta instalación**

El Software que utilize para la guía es:
  - VSCODE 1.65
  - Xdebug
  - xampp 3.2.24

**VS Code - PHP Debug**

Abrimos VSCODE, vamos a la pestaña extensiones, y buscamos lo siguiente:

![](assets/README-6e89b3ba.png)

Instalamos la aplicación

![](assets/README-7d1673e7.png)

Luego iremos a detalles de esa extensión y seleccionamos el enlace para ir xdebug

![](assets/README-d86af788.png)

Nos dirigira a esta pagina

![](assets/README-ca595c50.png)

**Xdebug**

A continuación vamos a xampp->phpinfo
![](assets/README-cc47566a.png)

seleccionamos todo el contenido de la página(ctrl+a) y lo copiamos

![](assets/README-e632d8be.png)

En la página de xdebug, vamos a pegar la informacion de phpinfo
![](assets/README-5c1957fd.png)

Pulsamos el boton analizar phpinfo(), y nos mostrara la informacion de nuestros servicios y las intrucciones para configurarlo

![](assets/README-08d59c71.png)

Ahora solo es seguir las instrucciones, primeramente seleccionamos el enlace de la primera opcion para descargar xdebug

![](assets/README-551079af.png)

Luego vamos a esta direccion C:\xampp\php\ext y pegamos el archivo descargado en esa carpeta

![](assets/README-b6d60cb9.png)

Luego paramos el servicio de apache en xampp

![](assets/README-c3030739.png)

Ahora en el panel de xampp iremos a la configuracion de apache

![](assets/README-f51d26e0.png)

Posteriormente seleccionamos la opcion php.ini, donde se nos abrira el fichero

![](assets/README-ea60292a.png)

Copiamos la siguiente linea donde se encuentra la ruta en mi caso sera la siguiente

> zend_extension = C:\xampp\php\ext\php_xdebug-3.1.3-8.1-vs16-x86_64.dll

En la parte final del fichero pegamos la linea copiada y guardamos
![](assets/README-8305846e.png)

Seguidamente para habilitar el debug remoto pegaremos en el fichero anterior tres lineas mas quedando el fichero así, y guardamos

![](assets/README-33acc804.png)

**VS Code - launch.json**

Nos vamos a VSCODE, creamos un archivo en la carpeta htdocs de xampp

![](assets/README-3eeb0296.png)

Ahora hacemos un pequeño programa de multiplicacion

![](assets/README-a2faadcf.png)

Nos vamos a la opcion de run and Debug

![](assets/README-43cfea14.png)


Seleccionamos el icono de configuración

![](assets/README-dd8a0e2b.png)

Nos aparecerá la siguiente ventana de configuración, donde copiaremos el siguiente contenido

![](assets/README-f2069d94.png)

Finalmente ya tenemos el debugger configurado.
