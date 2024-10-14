1. El directorio del proyecto contiene:
    - 5 ficheros HTML:
        a. 3 documentos con contenido, uno por ejercicio (higiene.html, lavado.html, riesgos.html)
        b. Documento de navegación, usado como índice (navigation.html)
        c. Documento principal, que integra los demás documentos en un HTML (index.html)
    - Directorio de recursos (imágenes) 'img/'
    - Hoja de estilos CSS 'styles.css'
    - README.txt - este documento, que trata de establecer los puntos principales del proyecto
    y facilitar la comprensión del razonamiento detrás de distintas soluciones. Cabe destacar que 
    este documento no documenta el código de una manera profesional. Además de este fichero, los 
    comentarios pueden servir para facilitar la comprensión también. 

2. El fichero 'index.html' utiliza los frames para combinar distintos HTMLs en un documento.
A la izquierda se puede observar el fichero de menu 'navigation.html', y a la derecha, el 
documento que corresponde con alguno de los ficheros HTML de contenido. Al pulsar el enlace 
correpondiente en el menu a la izquierda, el contenido de la página correspondiente aparece
en el marco de derecha.
  A la diferencia con los demas documentos, este utiliza HTML 4.01 con Frameset.
  Los marcos se definen mediante etiquetas <frame>, todos contenidas dentro de la etiqueta
<frameset>. Para evitar que un error imposibilite el uso de toda la página, se define el 
contenido alternativo dentro de la etiqueta <noframes>, con los anchors que apuntan a los 
ficheros HTML de contenido. 

3. El documento 'navigation.html' sirve de menu, contiene una serie de contenedores <div>, cada uno 
con un anchor que apunta a uno de los tres documentos de contenido.
  Utiliza estilos CSS definidos desde dentro del HTML, en la cabecera del documento mediante 
etiquetas <style>. 

4. El documento 'higiene.html' contiene la solución para el ejercicio 1. 
  Se explican algunas de las normas de higiene básica, con imágenes y textos explicativos.
Cada norma está contenida dentro de un contenedor <div>, con la clase 'norma', de lo que 
se hace uso para aplicar diseño al documento. 
  Las normas se ponen en filas con tres columnas, para lo que cada fila se define con un contenedor <div> 
con la clase 'contenedor-flex', llamado asi ya que en hoja de estilos se le aplica la propiedad 'display:flex'
con el fin de poner los elementos contenidos en el de una manera flexible, ajustando al espacio disponible.
Cada uno de estos contenedores contiene, por tanto, tres contenedores de clase 'norma'.
  La página también dispone de un footer con datos de contacto y un icono en formato SVG.
  Cabe destacar que ésta página utiliza diseños del CSS externo 'styles.css', con referencia al mismo 
en etiqueta <link rel="stylesheet">  dentro de <head> del documento.

