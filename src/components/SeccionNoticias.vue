<template>
  <section id="news" class="container-fluid mb-5">
    <div class="row">
    <div class="col-md-6 mb-4" v-for="(noticia, index) of noticias" :key="index">
      <img :src="noticia.urlToImage" width="100%"/>
      <h2>{{noticia.title}}</h2>
      <p>{{noticia.description}}</p>
      <div class="text-center">
      <a type="button" class="btn btn-primary" :href="noticia.url">Leer más</a>
      </div>
    </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "SeccionNoticias",
  data() {
    return {
      noticias: null,
    };
  },
  mounted() {
    const esperarAPI = async () => {
      let urlAPI =
        "https://newsapi.org/v2/top-headlines?country=co&category=business&apiKey=14e357be82684f2fba770db3fef54377";

      const obtenerAPI = await fetch(urlAPI, {
        method: "GET",
      });

      let resultadoAPI = await obtenerAPI.json();

      this.noticias = resultadoAPI.articles.slice(0, 4);

    };
    esperarAPI();
  },
};
</script>