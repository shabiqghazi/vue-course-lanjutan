<template>
  <div class="container mb-5">
    <h1 class="mb-4">Components</h1>
    <!-- <greet-component name="Shabiq Ghazi Arkaan" college-name="UIN Sunan Gunung Djati Bandung" />
    <greet-component name="Hendra Setiawan" college-name="Universitas Indonesia" />
    <greet-component :name="name" :college-name="collegeName" /> -->
    <!-- <article-component :class="['article-title', 'article-likes']" id="article-1" title="Tips lolos SNMPTN" :likes="50" :is-published="true" />
    <article-component class="article-title article-likes" id="article-2" title="Prediksi Soal UTBK 2023" :likes="1302" :is-published="true" /> -->
    <!-- <component-c /> -->
    <!-- <button class="btn btn-primary mb-3" @click="showPopup = true">show popup</button>
    <popup-component v-show="showPopup" @close="closePopup" /> -->
    <input-component v-model="name" />
  </div>
</template>

<script>
// import GreetComponent from "./components/GreetComponent.vue"
// import ArticleComponent from "./components/ArticleComponent.vue";
// import ComponentC from './components/ComponentC.vue'
// import PopupComponent from './components/PopupComponent.vue'
import InputComponent from "./components/Input.vue";

export default {
  name: "App",
  components: {
    // GreetComponent,
    // ArticleComponent,
    // ComponentC,
    // PopupComponent,
    InputComponent,
  },
  data() {
    return {
      // name: 'Anthony Sinisuka Ginting',
      // collegeName: 'Institut Teknologi Bandung',

      // showPopup: false,
      name: "",
    };
  },
  provide() {
    return {
      // username: this.name
    };
  },
  methods: {
    // closePopup(data){
    //   this.showPopup = false;
    //   console.log(data)
    // }
  },
};
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
