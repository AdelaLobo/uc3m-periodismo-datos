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

Lo siguiente es conseguir una cabecera y un pie por separado. Para ello edito el index desde nano y con ctrl+k elimino todas las líneas hasta quedarme solo con el código correspondiente, que en este caso son las primeras 71 y guardo el archivo como cabecera.html. Vuelvo abrir el index y con el mismo atajo me quedo con las últimas 15 líneas y lo guardo como pie.html. 

Como quiero que desde la parte superior el usuario se pueda dirigir a las diferentes prácticas, modifico la cabecera y el index de esta manera: 

    <li class="nav-item">
            <a class="nav-link" href="index.html">Inicio</a>
          </li>
          <li class="nav-item">
    <li class="nav-item">
            <a class="nav-link" href="nuevapractica1.html">Práctica 1</a>
          </li>
          <li class="nav-item">
    <li class="nav-item">
            <a class="nav-link" href="nuevapractica2.html">Práctica 2</a>
          </li>
          <li class="nav-item">
    <li class="nav-item">
            <a class="nav-link" href="nuevapractica3.html">Práctica 3</a>
          </li>
          <li class="nav-item">  
    <li class="nav-item">
            <a class="nav-link" href="nuevapractica4.html">Práctica 4</a>
         </li>
           <li class="nav-item">
     <li class="nav-item">
             <a class="nav-link" href="nuevametodologia.html">Metodología</a>

También edito la línea 44 para que se vea mi nombre en lugar de Fixed Navbar
    <a class="navbar-brand" href="#">Adela Lobo</a>

En el pie, modifico la línea 6 para introducir un nuevo texto. En este caso yo pondré *Periodismo de datos*. Quedaría de esta manera:
    <span class="text-muted">Periodismo de datos</span>

Para que la cabecera y el pie estén presentes durante toda la navegación debo concatenar. Para ello introduzco lo siguiente en la terminal:

 - cat cabecera.html practica1.html pie.html > nuevapractica1.html
 - cat cabecera.html practica2.html pie.html > nuevapractica2.html
 - cat cabecera.html practica3.html pie.html > nuevapractica3.html
 - cat cabecera.html practica4.html pie.html > nuevapractica4.html

Para que la página inicial tenga algo de texto, creo un nuevo archivo, al que he llamado inicio.md. En él, explico el contenido de la página web. Una vez terminado el texto lo paso a html con pandoc. Y copio y pego el contenido del nuevo archivo html en el index a partir del container. 

Ya solo me queda la metodología. Cuando termine de redactarla en markdown, le pasaré pandoc y con el comando cat uniré ese archivo con la cabecera y el pie. Guardaré este archivo como nuevametodología.html, que es la referencia que había introducido en la cabecera. 
