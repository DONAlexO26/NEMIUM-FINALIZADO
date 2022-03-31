____________________
*-----  QUE ES CSS  -----*
____________________

________________________________________

Cascading Style Sheets = Lenguaje de ESTILOS. 
________________________________________


SELECTORES


USER AGENT STYLE


COLORES


VALORES Y UNIDADES


PSEUDOCLASES


CUSTOM PROPERTIES


TIPOGRAFIA


BACKGROUND


PSEUDOELEMENTOS


CREAR COUNTERS


MODELO DE CAJA


    PROPIEDADES Y VALORES FISICOS

        Margenes
            Body= Margen predeterminado de 8px
            margin = Propiedad para modificar margenes 
                PRIMER FORMA DE MODIFICAR MARGENES:
                    margin-top:64px; = Propiedad que le da un valor de 64 pixels al margen superior
                    margin-bottom:64px; = Propiedad que le da un valor de 64 pixels al margen inferior
                    margin-right:10px; = Propiedad que le da un valor de de 10 pixels al margen derecho
                    margin-left: 10px; = Propiedad que le da un valor de 10 pixels al margen izquierdo
                SEGUNDA FORMA DE MODIFICAR MARGENES
                    margin: top right bottom left; = Declarar margenes para cada lado con tan solo una linea de codigo y una propiedad
                    EJEMPLO:
                        margin: 64px 10px 16px 32px; = Propiedad que da un valor de 64 pixels al margen de arriba - 10 pixels al margen de la derecha - 16 pixels al margen inferior - 32 pixels al margen izquierdo
                    OTROS CASOS
                         margin: 32px 10px 23px; =  Propiedad que da un valor de 32 pixels al margen superior - 10 pixels al margen derecho e izquierdo - 23 pixels al margen inferior
            HTML da margenes predeterminados a los elementos, estos margenes pueden verse desde el panel de inspeccionar en el apartado de Styles
            Cuando el valor es 0 no es necesario especificar nada, puesto que es un valor inexistente (NADA)

        Margin Collapsing
            Utilizar el panel de inspeccionar
            COLAPSO DE MARGENES = Cuando hay dos margenes en un mismo lugar
            LOS MARGENES NO SE SUMAN
            Aprender una buena logica respecto al margin collapsing
            El margin collapsing solamente funciona en un contexto de bloque (display:block;)
            Solamente funciona en vertical
            Horizontalmente los margenes se suman

        Padding
            Ligeramente parecido al margen, es una especie de relleno por dentro del elemento 
            padding = Propiedad para modificar el relleno de los elementos
            Las formas de modificar el relleno funciona igual al de modificar mergenes.

        Bordes
            Las formas de modificar el borde funciona igual al de modificar mergenes. 
            VALORES DEL BORDE: size type color
                EJEMPLO: border-left: 10px solid black; Borde a la izquiera con un tamaño de 10 pixeles de tipo solido y color negro.
                border-radius = redondear los bordes
                coordenadas del border radius (Esquina superior izquierda - Esquina superior derecha - Esquina inferior derecha - Esquina superior izquierda)
                EJEMPLO: border-radius: 50px 100px 10px 0; = Le da un radio de 50 pixels a la esquina superior izquierda, de 100 pixels a la esquina superior derecha, de 10 pixels a la esquina inferior derecha y de 0 pixels a la esquina inferior izquierda 


    PROPIEDADES Y VALORES FISICOS


BOX SIZING

    DAR TAMAÑOS A CONTENEDORES  O CAJAS
        widht = Ancho
        height = Altura
        border = Nos sirve para concer el area de nuestra caja
        El tamaño determinado de la caja por altura y ancho no es el resultado especifico, este resultado es la suma de padding x2 + border x2 
        El tamaño de la caja limita el contenido de si misma a su estructura = CONTENEDORES
        REGLA LOGICA PARA QUE EL TAMAÑO DE LA CAJA SEA EL DETERMINADO POR EL ANCHO Y ALTO: box-sizing: border-box;
        Ssaber usar el Box Sizing y no hacer que nos destruya


DEPURAR EN CSS

    Como estar seguro que mis selecetores son los correctos? 
    Ubicar el elemento tazando su caja al rededor
    !important para facilitar encontrar el elemento en el documento
    outline = Borde fuera del elemento que nos evita cualquier contratiempo en el documento
    box-shadow: RECIBEN 4 PARAMETROS; Parametros = Movimiento en el eje X - Movimiento en el eje Y - Cual va a sermi difuminado - spreet o color
    Parametro inset crea una sombra interna */

________________________________________________________________________________________________

LA TECNICA DEL WRAPPER
**SUPER IMPORTANTE**

    url  -   https://www.ionos.es/digitalguide/paginas-web/desarrollo-web/que-es-un-wrapper/
    url   -  https://developer.mozilla.org/es/docs/Learn/CSS/CSS_layout/Introduction
    Esta informacion esta contenida en el documento Marckdown  "./WRAPPER.md"

________________________________________________________________________________________________



POSICIONES
Propiedad = postion
La posicion por defecto es static (Elementos estaticos en el WebSite)
    
    position: relative;
        Se activan 5 propiedades [top left bottom right z-index]
        Fuciona como un margen (Empuje)
        Cuando el elemento se empuja = Su espacio natural no se ve alterado
        ¿Que es Z-index? Elementos encima de otros
            z-index= Dar valores a los elementos en un eje z (Profundidad) 
            Funciona similar a como se manejan las capas o layers en phothoshop.
            El z-index por defecto de los elementos es 1.
        
        position: absolute;
             Se activan 5 propiedades [top left bottom right z-index]
            Pierde el espacio fisico
            Se encima con el resto de cosas a partir de su posicion en el DOM
            Asi se hacen las ventanas de modal
            Los elementos son absolutos a algo pero relativos a otras cosas.
        MEZCLA DE POSICION RELATIVA Y ABSOLUTA
            Para limitar un elemento absoluto dentro de otro contenedor, el contenedor debe ser relativo

        position: fixed;
            Un position absolute fijo en la pantalla sin importar el scroll.

        position: sticky;
            Un position relative fijo en la pantalla sin importar el scroll.
            Para tomar la caracteristica de estar fijo en el sitio web, debemos otorgarle un valor y hacerlo relativo a algo (top: 0).



.
.
.
.
.

NOTAS EXTRA 

    <q></q> = Crear un quote en linea (Especificar una citacion en la semantica del dcumento) 
    <blockquote></blockquote> = Crear un quote en bloque (Especificar una citacion en la semantica del documento)

    display: none; propiedad de ocultar un elemento en el website, pero exsite en el HTML

    line-height: valor; propiedad para modificar el interlineado en un texto 

    <span></span> = Etiqueta para representar un contenido no semantico dentro de un contenido semantico, para diferenciar algun elemento en especial 