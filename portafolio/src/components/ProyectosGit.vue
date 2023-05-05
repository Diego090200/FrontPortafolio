<template>
    <!-- Contenedor para los 3 proyectos -->
    <div id="Proyectos" class="proyectos">
        <div class="titulo">Proyectos</div>
        <div class="proyecto">
            <!-- Contenedor para proyecto 1 -->
            <div class="proyecto1">
                <div class="cont-info">
                    <div class="subtitle">Spotify With R</div>
                    <div class="informacion">Este proyecto se realizó con el objetivo de obtener datos de una API proporcionada por Spotify, los datos obtenidos se almacenaron en data frames desde python, posteriormente fueron cargados y analizados con el lenguaje R, desde este se lograron obtener gráficas y estadísiticas. </div>
                    <!-- Contenedor para los botones -->
                    <div class="botones">
                        <input type="checkbox" id="btn-modal1">
                        <label for="btn-modal1" class="lbl-modal">Más Información</label>
                        <!-- Contenedor Informacion Modal Proyecto 1 -->
                        <div class="modal1">
                            <div class="contenedor1">
                                <header>Proyecto: Spotify With R</header>
                                <label for="btn-modal1">X</label>
                                <div class="contenido">
                                    <h4>Rol dentro del proyecto</h4>
                                    <p>Este proyecto se realizó para el curso de Análisis de datos, lo llevamos a cabo en parejas, para este proyecto se me asignó la tarea de crear los archivos csv a partir del json que conetenía la informacion recopilada de la API de spotify, posteriormente cargue el archivo csv a R y una base de datos en mongo, generé 2 Data Frame, uno desde el csv y otro realizando una conexion de mongo a R, a partir de estos Data Frame se generaron distintas gráficas estadísitcas para la discusion de resultados. </p>
                                    <h4>Proceso de creación</h4>
                                    <p>Inicialmente mi compañero extrajo la información de algunas playlist con Python por medio de una API de Spotify, los datos obtenidos se almacenaron en un archivo json, posteriormente almacene los datos del json en un archivo csv por medio de la libreria Pandas de Python, este csv se cargo a una base de datos no relacional en MongoDB, finalmente se realizaron las graficas desde R, estas gráficas se realizaron de los DataFrame creados a partir del archivo csv y por medio de una conexion a Mongo.</p>
                                    <h4>Resultado</h4>
                                    <p>Se obtuvieron resultados positivos de este proyecto, con este pude adquirir conocimentos para la conexion de aplicaciones con una API y la obtencion de información de la misma, además de amplir mis conocimientos respecto a Data Frame y el análisis de estos y finalmente los beneficios que nos provee el lenguaje R para el análisis estadístico.</p>
                                </div>
                            </div>
                        </div>
                        <button class="repositorio" onclick="window.open('https://github.com/Diego090200/Spotify-with-R ', '_blank');">
                            Repositorio
                            <img class="image2" src="/img/proyectos/github.png" alt="Videojuego RPG">
                        </button>
                    </div>
                </div>
                <img class="image1" src="/img/proyectos/SpotyR.png" alt="Spotify y R">
            </div>
            <!-- Contenedor para proyecto 2 -->
            <div class="proyecto2">
                <div class="cont-info">
                    <div class="subtitle">Youtube Web Scraping</div>
                    <div class="informacion">En este proyecto extraemos datos con python por medio de una API que nos provee Google que contiene distinta información de canales de YouTube, extrajimos datos de 10 canales de YouTube, posteriormente se almacenó la información en una BD relacional y una no relacional para posteriormente ser analizada por medio de un DWH.  </div>
                    <!-- Contenedor para los botones -->
                    <div class="botones">
                        <input type="checkbox" id="btn-modal2">
                        <label for="btn-modal2" class="lbl-modal">Más Información</label>
                        <!-- Contenedor Informacion Modal Proyecto 2 -->
                        <div class="modal2">
                            <div class="contenedor2">
                                <header>Proyecto: YouTube Web Scraping</header>
                                <label for="btn-modal2">X</label>
                                <div class="contenido">
                                    <h4>Rol dentro del proyecto</h4>
                                    <p>Este proyecto se realizó para el curso de Análisis de datos, lo llevamos a cabo en grupos de 4 personas, para este proyecto estuve encargado de la recopilación de datos de 3 canales de YouTube, tuve que consumir la API para poder obtener los datos, estuve a cargo de la creación de los QUERYS para almacenar la información recolectada en una base de datos relacional de MySql almacenada en un servidor en la nube. </p>
                                    <h4>Proceso de creación</h4>
                                    <p>El primer paso para este proyecto fue encontrar una API que nos brindara información de canales de YouTube, una vez establecida la API en este caso nos la provee Google, determinamos de los datos obtenidos los que nos podian ayudar para realizar una comparativa entre 10 canales, en este caso pudimos obtener vistas, comentarios y likes por video, recopilamos esta información por aproximadamente un mes, la información fue almacenada en una base de datos realcional y no relacional para hacer una comparación de los tiempos de carga, por la cantidad de datos pudimos crear una Big Data, con la información obtenida se creó un DWH con Pentaho y finalmente se crearon cubos para publicarlos y hacer un mejor analisis de la información recopilada.</p>
                                    <h4>Resultado</h4>
                                    <p>Pudimos determinar que para este tipo de datos las bases de datos no relacionales tienen mejores tiempos para la carga de información, al cabo de un mes pudimos recopilar millones de datos para formar nuestro Big Data y por medio de un DWH pudimos hacer un mejor analisis de la informacion obtenida.</p>
                                </div>
                            </div>
                        </div>
                        <button class="repositorio" onclick="window.open('https://github.com/Diego090200/Youtube_web_scaping', '_blank');">
                            Repositorio
                            <img class="image2" src="/img/proyectos/github.png" alt="Videojuego RPG">
                        </button>
                    </div>
                </div>
                <img class="image1" src="/img/proyectos/Yt.png" alt="Youtube x Python">
            </div>
            <!-- Contenedor para proyecto 3 -->
            <div class="proyecto3">
                <div class="cont-info">
                    <div class="subtitle">Video Juego RPG</div>
                    <div class="informacion">Se realizó un videojuego RPG programado en python con el objetivo de poner en práctica patrones y principios de diseño, el juego en si consta de 3 personajes elegibles por el jugador que combaten hasta agotar la barra de salud de cada contrincante, cada personaje posee distintas ventajas como más velocidad o más fuerza, además de que cuenta con 2 modos de juego, J1 vs J2 o un juego contra la máquina. </div>
                    <!-- Contenedor para los botones -->
                    <div class="botones">
                        <input type="checkbox" id="btn-modal3">
                        <label for="btn-modal3" class="lbl-modal">Más Información</label>
                        <!-- Contenedor Informacion Modal Proyecto 3 -->
                        <div class="modal3">
                            <div class="contenedor3">
                                <header>Proyecto: Video Juego RPG</header>
                                <label for="btn-modal3">X</label>
                                <div class="contenido">
                                    <h4>Rol dentro del proyecto</h4>
                                    <p>Este proyecto se realizó para el curso de Análisis y Diseño 2, lo llevamos a cabo en grupos de 4 personas, el objetivo de la práctica era implementar patrones de diseño en un videojuego, como equipo todos colaboramos para establecer los atributos y métodos de las clases y por medio de diagramas definir los patrones de diseño, en la parte de programación mi aporte fue para los eventos de movimiento de los personajes y el manejo de sus puntos de salud reflejados en la barra de HP. </p>
                                    <h4>Proceso de creación</h4>
                                    <p>Como grupo escogimos diseñar un videojuego RPG, este proyecto se desarrollo en Python y para la parte gráfica utilizamos PyGames, se definieron 3 tipos de personajes (Guerrero, Mago y Sanador)  y dos modos de juego que es jugador contra jugador y jugador contra la máquina (En este metodo solo hay 2 tipos de jugadores para la máquina que son Mob1 y Jefe), con esto establecido se creo el diagrama para el programa en donde se implemento el patrón de diseño de Factory Method para los tipos de Juego, ademas se definio una clase padre Personajes que heredaría sus atributos y métdos a cada clase de los personajes antes mencionados, finalmente se llevó a cabo el desarrollo del programa.</p>
                                    <h4>Resultado</h4>
                                    <p>Pudimos implementar correctamente el patrón de diseño de Factory Method, con esto logramos aplicar algunos de los principios SOLID, como por ejemplo el principio de Responsabilidad Unica (S), el principio de Abierto/Cerrado (O) y el principio de Liskov (L), además de trabajar nuestro código ordenado y tipado con PEP8.</p>
                                </div>
                            </div>
                        </div>
                        <button class="repositorio" onclick="window.open('https://github.com/Diego090200/Videojuego-RPG ', '_blank');">
                            Repositorio
                            <img class="image2" src="/img/proyectos/github.png" alt="Videojuego RPG">
                        </button>
                    </div>
                </div>
                <img class="image1" src="/img/proyectos/rpg.png" alt="Videojuego RPG">
            </div>
        </div>
    </div>
    
</template>

<style scoped>
    /* Estilos para contenedor de proyectos*/
    .proyectos{
        align-items: center;
        color: #FFFFFF;
        display: flex;
        flex-direction: column;
        font-family: 'Nunito', sans-serif;
        font-style: normal;
        justify-content: center;
        line-height: 1.3em;
        margin-top: 5%;
    }

    /* Estilos para el titulo*/
    .titulo{
        font-size: 2.7em;
        line-height: 2.5em; 
        margin-bottom: 10px;
        text-decoration: underline wavy;
        text-decoration-color: #2C66C3;
    }

    /* Estilos para contenedor de los 3 proyectos*/
    .proyecto{
        align-items: center;
        display: flex;
        flex-direction: column;
        flex-direction: column;
        margin-bottom: 5%;
    }

    /* Estilos para contenedor de cada proyecto*/
    .proyecto1, .proyecto3, .proyecto2{
        align-items: center;
        display: flex;
        flex-direction: row;
        gap: 5%;
        justify-content: center;
    }

    /* Cambio de direccion unicamente para el proyecto 2*/
    .proyecto2{
        flex-direction: row-reverse;
    }

    /* Margen para proyecto 2 y 3*/
    .proyecto2, .proyecto3{
        margin-top: 7%;
    }

    /* Estilos para contenedor de los botones*/
    .botones{
        align-items: center;
        display: flex;
        flex-direction: row;
        justify-content: space-around;
        margin-top: 5%;
        width: 100%;
    }

    /* Estilos para el boton que muestra caja modal*/
    #btn-modal1, #btn-modal2, #btn-modal3{
        display: none;
    }
    /* Desplegar cada ventana modal segun el proyecto selecionado*/
    #btn-modal1:checked ~ .modal1, #btn-modal2:checked ~ .modal2, #btn-modal3:checked ~ .modal3{
        opacity: 1;
        visibility: visible;
    }

    /* Estilos para el boton mas informacion*/
    .lbl-modal{
        background: #2C66C3;
        padding: 0.8% 1%;
        border-radius: 4px;
        cursor: pointer;
        width: 40%;
        height: 2.2em;
        flex-direction: row;
        display: flex;
        color: #FFFFFF;
        align-items: center;
        justify-content: center;
    }

    /* Estilos para caja modal que muestra informacion de educacion*/
    .modal1, .modal2, .modal3{
        width: 100%;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        position: fixed;
        top: 0;
        left: 0;
        background: rgba(0, 0, 0, 0.5);
        transition: all 500ms ease;
        opacity: 0;
        visibility: hidden;
    }

    .contenedor1, .contenedor2, .contenedor3 {
        width: 60%;
        height: 70%;
        margin: auto;
        background: #293548;
        box-shadow: 1px 7px 25px rgba(0, 0, 0, 0.6);
        transition: all 500ms ease;
        position: relative;
        transform: translateY(-30%);
        overflow-y: scroll;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .contenedor1::-webkit-scrollbar, .contenedor2::-webkit-scrollbar, .contenedor3::-webkit-scrollbar{
        width: 10px;
    }
    .contenedor1::-webkit-scrollbar-thumb, .contenedor2::-webkit-scrollbar-thumb, .contenedor3::-webkit-scrollbar-thumb{
        background: #4b4f54;
        border-radius: 10%;
    }

    /* Animacion de despliegue para ventana modal*/
    #btn-modal1:checked ~ .modal1 .contenedor1, #btn-modal2:checked ~ .modal2 .contenedor2, #btn-modal3:checked ~ .modal3 .contenedor3{
        transform: translateY(0%);
    }


    .contenedor1 header, .contenedor2 header, .contenedor3 header{
        padding: 1%;
        background: #222d3a;
        color: #FFFFFF;
        width: 98%;
        font-weight: 600;
    }

    .contenedor1 label, .contenedor2 label, .contenedor3 label{
        position: absolute;
        top: 10px;
        right: 10px;
        color: #FFFFFF;
        font-size: 15px;
        cursor: pointer;
    }

    .contenido{
        margin-top: 2%;
        margin-bottom: 2%;
        width: 93%;
        background-color: #506d8b;
    }
    .contenido p{
        margin: 3%;
        display: flex;
        text-align: justify;
    }
    
    /* Estilos para el boton que redirecciona al proyecto de git*/
    .repositorio{
        align-items: center;
        background-color: transparent;
        border-color: #FFFFFF;
        border-radius: 4px;
        color: #FFFFFF;
        display: flex;
        flex-direction: row;
        height: 3.5em;
        justify-content: space-around;
        padding: 1em;
        width: 40%;
    }

    /* Estilos para el contenedor de la informacion del proyecto*/
    .cont-info{
        align-items: center;
        display: flex;
        flex-direction: column;
        gap: 5%;
        justify-content: center;
        padding: 20px;
        text-align: center;
        width: 40%;
    }

    /* Estilos para los subtitulos*/
    .subtitle{
        margin-bottom: 5%;
        font-size: 2em;
    }

    /* Estilos para el texto de la informacion*/
    .informacion{
        display: flex;
        flex-direction: column;
        font-size: 1em;
        margin-bottom: 5%;
        text-align: justify;
    }

    .image1{
        width: 18%;
        height: 18%;
    }

</style>