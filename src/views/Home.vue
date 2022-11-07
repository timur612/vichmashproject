<template>
  <div class="">
    <p class="h1 mt-3" style="margin-left:5%">Беспроводные сети</p>

    <div class="d-flex" style="margin-left:5%;height:2.5rem">
     <div class="vr" style="width:0.2rem;opacity:100%" ></div>
    </div>

    <div>
      <div class="position-absolute" style="top:15%;left:3%">
        <p class="h3" style="cursor:pointer" v-on:click="()=>this.$router.push('/about')">Все про WiFi</p>
      </div>
      <div class="mt-5 d-flex" style="margin-left:5%;height:31rem">
        <div class="vr" style="width:0.2rem;opacity:100%" ></div>
      </div>
      <div class="position-absolute" style="top:15%;left:88%">
        <p class="h3" style="cursor:pointer" v-on:click="()=>this.$router.push('/page2')">Точки доступа</p>
      </div>
      <div id="main_img" class="position-absolute top-50 start-50 translate-middle">
            <img class="main_img" alt="Vue logo" src="../assets/icon.png">
      </div>
      <div class="position-absolute" style="top:90%;left:3%">
        <p class="h3" style="cursor:pointer">Роутеры</p>
      </div>

      <div class="position-absolute d-flex" style="top:41rem;left:11rem;">
        <div class="hr"></div>
      </div>

      <div class="position-absolute" style="top:90%;left:88%">
        <p class="h3" style="cursor:pointer">Ссылка 4</p>
      </div>

      <div class="position-absolute d-flex" style="top:11rem;left:90rem;">
        <div class="vr" style="height:29rem;width:0.2rem;opacity:100%" ></div>
      </div>

      <div class="position-absolute d-flex" style="top:4rem;left:90rem;">
        <div class="vr" style="height:3rem;width:0.2rem;opacity:100%" ></div>
      </div>

      <div class="position-absolute d-flex" style="top:2.8rem;left:5rem;">
        <div class="hr" style="width:85rem"></div>
      </div>

    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import anime from 'animejs/lib/anime.es.js';

export default {
  name: 'Home',
  components: {
    
  },
  methods:{
  }
}
</script>

<style scoped>
  .hr {
   margin: 1rem 0;
    color: inherit;
    background-color: currentColor;
    border: 0;
    width:73rem;
    height: 0.2rem;
  }
</style>
