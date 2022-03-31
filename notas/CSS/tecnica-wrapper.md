________________________________________________________________________________________________

LA TECNICA DEL WRAPPER
**SUPER IMPORTANTE**

    url  -   https://www.ionos.es/digitalguide/paginas-web/desarrollo-web/que-es-un-wrapper/
    url   -  https://developer.mozilla.org/es/docs/Learn/CSS/CSS_layout/Introduction
    Esta informacion esta contenida en el documento Marckdown  "./WRAPPER.md"

________________________________________________________________________________________________

Arquitectura escalable para proyectos sencillos y proyectos sofisticados.

LANDPAGE = Infalible

Envolver el contenido
    Elementos de Bloque (Main - Div - Secition ....)
    Los elementos de bloque, pueden centrarse con [margin: auto;]
    Widht = Dar ancho al bloque (Contenedor/Wrapper)
    No meter todo en una caja
        CONSEJO: Trabajar por secciones
        Tener una .clase por contenedor
    Ejemplo: 
    <main class="main">  Bloque que representa el contenido principal del body - Crear seguridad en los elementos.
        <div class="wrapper"> Contendor para editar tamaño y posicion
            <div class=main-content> Contenedor que representa el contenido incluido dentro del .Wrapper
                Contenido de la pagina web
            <div class=main-content> Contenedor que representa el contenido incluido dentro del .Wrapper
        <div class="wrapper">Contendor para editar tamaño y posicion
    <main class="main">  Bloque que representa el contenido principal del body - Crear seguridad en los elementos.

>   Ejemplo mas completo

<main class="main"><!--Es el contenedor base padre de todas las cosas -->
  <div class="wrapper">
    <div class="main-content">
      <section class="section-setup">
        <div class="wrapper">
          <div class="setup-content">
          </div>
        </div>
      </section>
      <section class="section-des-web">
        <div class="wrapper">
          <div class="des-web-content">
          </div>
        </div>
      </section>
      <section class="section-box-model">
        <div class="wrapper">
          <div class="box-model-content">
          </div>
        </div>
      </section>
    </div>
  </div>
</main>

    

