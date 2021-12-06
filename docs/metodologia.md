# Metodología
Estamos a punto de acabar el cursos y, por tanto, voy a recopilar todo el trabajo de este cuatrimestre en este página web.
Para ello, voy a necesitar crear la carpeta docs, ya que github me creará la web con todo el contenido que aparezca ahí. Es tan fácil como introducir en la terminal **mkdir docs**. Como también voy a necesitar otras dos carpetas para los archivos css y js, repito el proceso anterior. Introduco **mkdir css** y **mkdir js**

Ya tengo cuatro archivos en markdown y cada uno corresponde a una práctica del curso. Para insertarlos en una página web debo pasarlos a html.
Este paso es bien sencillo, tan solo debo introducir en la terminal la siguiente fórmula: **pandoc ruta/archivo.md ruta/nuevoarchivo.html**.
En mi caso, puse esto en la terminal:
 
- pandoc uc3m-periodismo-datos/docs/practica1.md uc3m-periodismo-datos/docs/practica1.html
- pandoc uc3m-periodismo-datos/docs/Practica2.md uc3m-periodismo-datos/docs/practica2.html
- pandoc uc3m-periodismo-datos/docs/Practica3.md uc3m-periodismo-datos/docs/practica3.html
- pandoc uc3m-periodismo-datos/docs/Grafico2.md uc3m-periodismo-datos/docs/practica4.html

Ya tengo todos los archivos en html. Ahora falta crear una web para insertarlos. Por ello, descargo una plantilla html de **Bootstrap**. En su web, en la pestaña *Examples*, clico en *Download examples* y me descargo las plantillas. 

Para acceder al index de la plantilla stiky footer navbar introduzco en la terminal cd /Downloads/bootstrap-5.1.3-examples/bootstrap-5.1.3-examples/sticky-footer-navbar. Ahora puedo modificar el archivo index.html con nano. Pero como no me interesa tenerlo en esta carpeta lo muevo a la carpeta docs de mi directorio con mv. También muevo a la carpeta css los archivos bootstrap.min.css y sticky-footer-navbar.css. Realizo el mismo proceso para mover a la carpeta js bootstrap.bundle.min.js. 

Listo, ya tengo todo lo necesario para empezar a modificar el index. Aquí voy a tener que cambiar algunas rutas para que el diseño de la web sea atractivo.´Cambio dos rutas de la cabecera del index en las que aparece un archivo css. De tal manera que las rutas modificadas quedarían así: 
  
**<link href="css/bootstrap.min.css" rel="stylesheet">**

    **<link href="css/sticky-footer-navbar.css" rel="stylesheet">**

En el pie del index debo cambiar la ruta de otro archivo js. El resultado de la nueva ruta sería el siguiente:

    **<link href="css/sticky-footer-navbar.css" rel="stylesheet">**




