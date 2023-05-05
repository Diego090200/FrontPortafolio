<template>
    <div id="Inicio" class="inicio">
        <div class="contenedor">
            <div class="informacion">
                <div class="hola">Hola, soy</div>
                <div class="name">Diego Hernández</div>
                <div class="carrera">&lt;Ingeniero en informática y sistemas/&gt;</div>
                <div class="description">Soy una persona con deseos de superación y disposición para el aprendizaje. Poseo habilidades para diseño web, organización, planificación y trabajar en equipo. Me considero alguien proactivo, dinámico, responsable y con excelentes relaciones humanas.</div>
            </div>
            <img class="perfil" src="/img/Perfil.jpg" alt="Imagen de Perfil">
        </div>
    </div>
</template>

<style scoped>
    .inicio{
        display: flex;
        justify-content: center;
        align-items: center;
        padding: 5vw 2vw;
        font-family: "Nunito", sans-serif;
        font-style: normal;
    }

    .contenedor{
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 5vw;
        width: 90%;
    }

    .informacion{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        max-width: 50%;
        width: 100%;
    }

    .hola{
        font-weight: 400;
        font-size: 2.5vw;
        line-height: 1.5;
        text-align: center;
        color: #ffffff;

        display: flex;
        align-items: center;
        text-align: center;
        flex-direction: column;
    }

    .name{
        font-weight: 400;
        font-size: 4vw;
        line-height: 1.2;

        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;

        color: #FFFFFF;
    }

    .carrera{
        font-weight: 400;
        font-size: 2.2vw;
        line-height: 1.2;

        display: flex;
        align-items: center;
        flex-direction: column;

        color: #2CB67D;
    }

    .description{
        font-weight: 400;
        font-size: 20px;
        line-height: 23px;
        text-align: justify;

        display: flex;
        flex-direction: column;
        color: #FFFFFF;
    }

    .perfil{
        border-radius: 50%;
        height: 30%;
        width: 30%;
    }
</style>