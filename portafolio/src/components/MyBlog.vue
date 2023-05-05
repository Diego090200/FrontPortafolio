<template>
  <div class="myblog" id="MyBlog">
    <div v-if="error">
      {{ error }}
    </div>
    <header class="titulo">
      Mi Blog
    </header>
    <p class="info-blog">
      ¡Bienvenido a mi blog sobre desarrollo de aplicaciones y artículos para ingeniería en sistemas! Me complace tener la oportunidad de compartir mis conocimientos y experiencia en el campo de la programación y la ingeniería de software con ustedes, espero que de esta manera puedan conocerme mejor.
    </p>
    <input type="checkbox" id="btn-modal-blog">
    <label for="btn-modal-blog" class="lbl-modal">Ver Entradas del Blog</label>         
    <!-- Contenedor para modal de informacion académica -->
    <div id="Modal-Blog" class="modal">
      <div class="contenedor">
          <header>Mi Blog</header>
          <label for="btn-modal-blog">X</label>
          <div class="contenido" v-for="post in posts" :key="post.id">
            <h4 class="blog-title">{{ post.attributes.Title }}</h4>
            <p class="blog-content">{{ post.attributes.Content }}
              <img class="image" src="/img/blog/front-blog.png" alt="Imagen Desarrollo Front">
            </p>
                
          </div>
      </div>
    </div>
  </div>
</template>
<script>
import axios from 'axios'

export default {
name: 'MyBlog',
data () {
  return {
    posts: [],
    error: null
  }
},
async mounted () {
  try {
    const response = await axios.get('http://localhost:1337/api/posts/?populate=*', {
      headers: {
          Authorization: 'Bearer fcfd1e606ad23e14f4453f3f098a156f42e3f2cf484a55ca198a5e1b72aed825a2d7917ee31e870d2b1e1c775a4dba66cdcecf7370ab43b163bc2d07df9f9575dd42f214308adbc4f3fe84b85561d39af4d55cc01c46a5c2fb694aeee5093ec539295689909ecbf79f653d0843a65a05c4052f95d467440416bcf5b871bcdd43'
      },
    });
    this.posts = response.data.data;
  } catch (error) {
    this.error = error;
  }
}
}
</script>
<style scoped>
.myblog {
  align-items: center;
  color: #FFFFFF;
  display: flex;
  flex-direction: column;
  font-family: 'Nunito', sans-serif;
  font-style: normal;
  line-height: 1.3em;
  margin-top: 5%;
}

/* Estilos para titulo*/
.titulo{
  font-size: 2.7em;
  line-height: 2.5em; 
  margin-bottom: 10px;
  text-decoration: underline wavy;
  text-decoration-color: #2C66C3;
}

.info-blog{
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
#btn-modal-blog {
  display: none;
}

#btn-modal-blog:checked~.modal {
  opacity: 1;
  visibility: visible;
}

.lbl-modal {
  background: #2C66C3;
  border-radius: 4px;
  cursor: pointer;
  padding: 0.8% 1%;
}

/* Estilos para caja modal que muestra informacion de educacion*/
.modal {
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

.contenedor {
  align-items: center;
  background: #293548;
  box-shadow: 1px 7px 25px rgba(0, 0, 0, 0.6);
  display: flex;
  flex-direction: column;
  height: 85%;
  margin: auto;
  overflow-y: scroll;
  position: relative;
  transform: translateY(-30%);
  transition: all 500ms ease;
  width: 90%;
}

.contenedor::-webkit-scrollbar {
  width: 10px;
}

.contenedor::-webkit-scrollbar-thumb {
  background: #4b4f54;
  border-radius: 10%;
}

#btn-modal-blog:checked~.modal .contenedor {
  transform: translateY(0%);
}

.contenedor header {
  background: #222d3a;
  color: #FFFFFF;
  padding: 1%;
  width: 98%;
  font-weight: 600;
}

.contenedor label {
  color: #FFFFFF;
  cursor: pointer;
  font-size: 15px;
  position: absolute;
  right: 10px;
  top: 10px;
}

.contenido p{
      margin: 3%;
      display: flex;
      text-align: justify;
  }

/* Estilos para contenido del modal*/

.contenido {
  background-color: #506d8b;
  margin-bottom: 2%;
  margin-top: 2%;
  width: 93%;
}

.blog-content .image {
  width: 30%;
  height: 20%;
  margin: 0;
  align-self: center;
}

.blog-content {
  display: flex;
  flex-direction: column;
}

</style>