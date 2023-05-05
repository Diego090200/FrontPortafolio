<template>
  <NavBar></NavBar>
  <inicio-presentacion></inicio-presentacion>
  <ProyectosGit></ProyectosGit>
  <edu-habilidad></edu-habilidad>
  <my-blog></my-blog>
  <contacto-redes></contacto-redes>
</template>

<script>
import ContactoRedes from './components/Contacto-Redes.vue';
import InicioPresentacion from './components/InicioPresentacion.vue';
import NavBar from './components/NavBar.vue';
import EduHabilidad from './components/Edu-Habilidad.vue';
import ProyectosGit from './components/ProyectosGit.vue';
import MyBlog from './components/MyBlog.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    InicioPresentacion,
    ContactoRedes,
    EduHabilidad,
    ProyectosGit,
    MyBlog
}
}
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: #111827;
  min-height: 100vh;
}
body{
  margin: 0; 
  padding: 0;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: #111827;
  min-height: 100vh;
}
</style>
