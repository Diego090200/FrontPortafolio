<template>
    <div id="Educacion" class="educacion-habilidad">
        <!-- Contenedor para la informacion respecto a educacion -->
        <div class="educacion">
            <div class="titulo">
                Educación
            </div>
            <div class="edu-info">
                Actualmente estoy terminando mis estudios universitarios en la Universidad Rafael Landivar, Campus de Quetzaltenango, en el trayecto de mi vida educativa e desarrollado habilidades para el diseño de aplicaciones web y de escritorio, personalmente se me facilita el trabajo en equipo y la comunicación con mis compañeros.
            </div>
            <input type="checkbox" id="btn-modal">
            <label for="btn-modal" class="lbl-modal">Más Información</label>         
            <!-- Contenedor para modal de informacion académica -->
            <div class="modal">
                <div class="contenedor">
                    <header>Información Académica</header>
                    <label for="btn-modal">X</label>
                    <div class="contenido">
                        <ul class="listado-logros">
                            <li><a>Participación del curso de Docker desde 0 impartido por la empresa LaserAnts de Quetzaltenango.</a></li>
                            <li><a>Participación en la conferencia de parte de ESET Antivirus, acerca de la Seguridad en Dispositivos.</a></li>
                            <li><a>Participación en el XV Simposio de Ingeniería denominado Ingeniería que transforma al mundo, Universidad Rafael Landívar Campus de Quetzaltenango.</a></li>
                            <li><a>Participación en el XIV Simposio de Ingeniería denominado Evolución para trascender, Universidad Rafael Landívar Campus de Quetzaltenango.</a></li>
                            <li><a>Participación en el XIII Simposio de Ingeniería denominado Innovación, retos y oportunidades, Universidad Rafael Landívar Campus de Quetzaltenango.</a></li>
                            <li><a>Participación en el XII Simposio de Ingeniería denominado Ingenio y optimización, Universidad Rafael Landívar Campus de Quetzaltenango.</a></li>
                            <li><a>Participación en el XI Simposio de Ingeniería sobre la Calidad en la Ingeniería, Universidad Rafael Landívar Campus de Quetzaltenango.</a></li>
                            <li><a>Participación en el taller de parte de Señor Xplorer, acerca de Reparación de Computadores y conexiones web.</a></li>
                            <li><a>Participación en el XII Simposio de Ingeniería denominado Ingenio y optimización, Universidad Rafael Landívar Campus de Quetzaltenango.</a></li>
                            <li><a>Participación en el XI Simposio de Ingeniería sobre la Calidad en la Ingeniería, Universidad Rafael Landívar Campus de Quetzaltenango.</a></li>
                            <li><a>Participación en el taller de parte de Señor Xplorer, acerca de Reparación de Computadores y conexiones web.</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
        <!-- Contenedor para la informacion respecto a mis habilidades -->
        <div class="habilidades">
            <div class="titulo">
                Habilidades
            </div>
            <div class="habilidades-info">
                <div class="html">
                    <img src="/img/tecnologias/html.png" alt="HTML" class="logo-tecnologia">
                    HTML
                </div>
                <div class="css">
                    <img src="/img/tecnologias/css.png" alt="CSS" class="logo-tecnologia">
                    CSS
                </div>
                <div class="typescript">
                    <img src="/img/tecnologias/typescript.png" alt="TS" class="logo-tecnologia">
                    TypeScript
                </div>
                <div class="javascript">
                    <img src="/img/tecnologias/javascript.png" alt="JS" class="logo-tecnologia">
                    JavaScript
                </div>
                <div class="react">
                    <img src="/img/tecnologias/reactjs.png" alt="React" class="logo-tecnologia">
                    React
                </div>
                <div class="vue">
                    <img src="/img/tecnologias/vue.png" alt="Vue" class="logo-tecnologia">
                    Vue
                </div>
                <div class="java">
                    <img src="/img/tecnologias/Java.png" alt="Java" class="logo-tecnologia">
                    Java
                </div>
                <div class="python">
                    <img src="/img/tecnologias/Python.png" alt="Python" class="logo-tecnologia">
                    Python
                </div>
                <div class="mongo">
                    <img src="/img/tecnologias/mongodb.png" alt="MongoDB" class="logo-tecnologia">
                    MongoDB
                </div>
                <div class="mysql">
                    <img src="/img/tecnologias/mssql.png" alt="MySQL" class="logo-tecnologia">
                    MySQL
                </div>
                <div class="git">
                    <img src="/img/tecnologias/git.png" alt="Git" class="logo-tecnologia">
                    Git
                </div>
                <div class="figma">
                    <img src="/img/tecnologias/figma.png" alt="Figma" class="logo-tecnologia">
                    Figma
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped>
    /* Estilos para el contenedor de educacion y habilidades*/
    .educacion-habilidad{
        align-items: center;
        color: #FFFFFF;
        display: flex;
        flex-direction: column;
        font-family: 'Nunito', sans-serif;
        font-style: normal;
        line-height: 1.3em;
        margin-top: 5%;
    }

    /* Estilos para el contenedor de educacion*/
    .educacion{
        align-items: center;
        display: flex;
        flex-direction: column;
        gap: 5%;
        justify-content: center;
        padding: 10px;
        width: 100%;
    }

    /* Estilos para la informacion de la educacion*/
    .edu-info{
        align-items: center;
        display: flex;
        flex-direction: row;
        font-size: 1.5em;
        gap: 5%;
        height: 10%;
        justify-content: center;
        line-height: 120%;
        padding: 1%;
        text-align: justify;
        width: 70%;
    }

    /* Estilos para el boton que muestra caja modal*/
    #btn-modal{
        display: none;
    }
    #btn-modal:checked ~ .modal{
        opacity: 1;
        visibility: visible;
    }
    .lbl-modal{
        background: #2C66C3;
        border-radius: 4px;
        cursor: pointer;
        padding: 0.8% 1%;
    }

    /* Estilos para caja modal que muestra informacion de educacion*/
    .modal{
        align-items: center;
        background: rgba(0, 0, 0, 0.5);
        display: flex;
        height: 100vh;
        justify-content: center;
        left: 0;
        opacity: 0;
        position: fixed;
        top: 0;
        transition: all 500ms ease;
        visibility: hidden;
        width: 100%;
    }

    .contenedor{
        align-items: center;
        background: #293548;
        box-shadow: 1px 7px 25px rgba(0, 0, 0, 0.6);
        display: flex;
        flex-direction: column;
        height: 70%;
        margin: auto;
        overflow-y: scroll;
        position: relative;
        transform: translateY(-30%);
        transition: all 500ms ease;
        width: 60%;
    }
    .contenedor::-webkit-scrollbar{
        width: 10px;
    }
    .contenedor::-webkit-scrollbar-thumb{
        background: #4b4f54;
        border-radius: 10%;
    }

    #btn-modal:checked ~ .modal .contenedor{
        transform: translateY(0%);
    }

    .contenedor header{
        background: #222d3a;
        color: #FFFFFF;
        padding: 1%;
        width: 98%;
    }

    .contenedor label{
        color: #FFFFFF;
        cursor: pointer;
        font-size: 15px;
        position: absolute;
        right: 10px;
        top: 10px;
    }

    /* Estilos para contenido del modal*/

    .contenido{
        background-color: #506d8b;
        margin-bottom: 2%;
        margin-top: 2%;
        width: 93%;
    }
    .listado-logros{
        display: flex;
        flex-direction: column;
        margin: 4% 2% 4% 3%;
        text-align: start;
    }

    /* Estilos para los titulos*/
    .titulo{
        font-size: 2.7em;
        line-height: 2.5em; 
        margin-bottom: 10px;
        text-decoration: underline wavy;
        text-decoration-color: #2C66C3;
    }

    /* Estilos para el contenedor de habilidades*/
    .habilidades{
        align-items: center;
        display: flex;
        flex-direction: column;
        justify-items: center;
        margin-top: 10%;
        margin-bottom: 15%;
        width: 100%;
    }

    /* Estilos para las tecnologias de habilidades*/
    .habilidades-info{
        align-items: center;
        display: grid;
        font-size: 32px;
        grid-template-columns: repeat(4, 25%);
        grid-template-rows: 60.31% 60.31% 60.31%;
        justify-items: center;
        margin-top: 1%;
        width: 70%;
    }

    /* Posicionamiento para las tecnologias en el grid*/
    .html {
        grid-column: 1;
        grid-row: 1;
    }
    .css{
        grid-column: 2;
        grid-row: 1;
    }
    .typescript{
        grid-column: 3;
        grid-row: 1;
    }
    .javascript{
        grid-column: 4;
        grid-row: 1;
    }
    .react{
        grid-column: 1;
        grid-row: 2;
    }
    .vue{
        grid-column: 2;
        grid-row: 2;
    }
    .java{
        grid-column: 3;
        grid-row: 2;
    }
    .python{
        grid-column: 4;
        grid-row: 2;
    }
    .mongo{
        grid-column: 1;
        grid-row: 3;
    }
    .mysql{
        grid-column: 2;
        grid-row: 3;
    }
    .git{
        grid-column: 3;
        grid-row: 3;
    }
    .figma{
        grid-column: 4;
        grid-row: 3;
    }

    /* Estilos para los contenedores de cada tecnologia*/
    .html, .css, .typescript, .javascript, .react, .vue, .java, .python, .mongo, .mysql, .git, .figma{
        align-items: center;
        border-radius: 8px;
        border: 3px solid #293548;
        display: flex;
        height: 60px;
        justify-content: center;
        width: 75%;
        font-size: 85%;
    }

    /* Definicion de tamaño para las imagenes de las tecnologias*/
    .logo-tecnologia{
        height: 35px;
        margin-right: 2px;
        width: 35px;
    }
</style>