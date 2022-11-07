<template>
  <div class="about">
    <div class="position-absolute top-0 start-0" v-on:click="()=>this.$router.push('/')"><img style="width:10%;cursor:pointer" src="../assets/back.png" alt=""></div>
    <div class="m-5" style="width:43%">
      <p class="h2">Wifi</p>
      <div class="mt-3">
        <div class="border rounded p-2" style="font-size:1.2rem">
          <p>Wi-Fi — технология беспроводной локальной сети с устройствами на основе стандартов IEEE 802.11. 
          Wi-Fi был создан в 1997 году в лаборатории радиоастрономии CSIRO в Канберре, Австралия.</p>
          
          <p>Основными диапазонами Wi-Fi считаются 2,4 ГГц, 5 ГГц и 6 ГГц. При частоте в 2,4 ГГц максимальная скорость Wi-Fi 11 Мбит/с</p>
        </div>
        <p class="h4 mt-3">Базы стандартов</p>
        <div class="border rounded p-2" style="font-size:1.2rem">
          <p>набор стандартов  связи для коммуникации в беспроводной локальной сетевой зоне частотных диапазонов 0,9; 2,4; 3,6; 5 и 60 ГГц.</p>
        </div>
      </div>
    </div>
    
    <img class="main_img position-absolute" alt="Vue logo" src="../assets/icon.png">
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
    getTolink(){
      anime({
        targets: '.main_img',
        width: '90%',
        // marginLeft:'50%',
        left:'50%',
        top:'5%',
        height: 'auto',
        opacity:'50%'
      })
    }
  },
  mounted(){
    this.getTolink();
  }
}
</script>

<style scoped>
  .main_img{
    position:'absolute';
  }
</style>