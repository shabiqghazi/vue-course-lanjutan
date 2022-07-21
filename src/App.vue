<template>
  <div class="container mb-5">
    <h1 class="mb-4">Components</h1>
    <!-- <greet-component name="Shabiq Ghazi Arkaan" college-name="UIN Sunan Gunung Djati Bandung" />
    <greet-component name="Hendra Setiawan" college-name="Universitas Indonesia" />
    <greet-component :name="name" :college-name="collegeName" /> -->
    <!-- <article-component :class="['article-title', 'article-likes']" id="article-1" title="Tips lolos SNMPTN" :likes="50" :is-published="true" />
    <article-component class="article-title article-likes" id="article-2" title="Prediksi Soal UTBK 2023" :likes="1302" :is-published="true" /> -->
    <component-c />
  </div>
</template>

<script>
// import GreetComponent from "./components/GreetComponent.vue"
// import ArticleComponent from "./components/ArticleComponent.vue";
import ComponentC from './components/ComponentC.vue'

export default {
  name: 'App',
  components: {
    // GreetComponent,
    // ArticleComponent,
    ComponentC
  },
  data(){
    return {
      name: 'Anthony Sinisuka Ginting',
      collegeName: 'Institut Teknologi Bandung'
    }
  },
  provide(){
    return {
      username: this.name
    }
      
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
