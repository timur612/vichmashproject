<template>
  <div class="about">
    <div class="position-absolute top-0 start-0" v-on:click="()=>this.$router.push('/')"><img style="width:10%;cursor:pointer" src="../assets/back.png" alt=""></div>
    <div class="container mt-4" style="margin-left:50%;width:50%;">
      <p class="h2">Точки доступа и их режимы работы </p>
      <div class="mt-3">
        <div class="border rounded p-2" style="font-size:1.2rem">
            <p>Точка доступа (точка беспроводного доступа) — это сетевое устройство, которое позволяет подключать совместимые устройства к сети беспроводной связи. Такое устройство может быть либо физически связано с маршрутизатором, либо встроено в него.</p>
            <p>Радиус действия стандартной точки доступа – примерно 200-250 метров, при условии, что на этом расстоянии не будет никаких препятствий.</p>
        </div>
        <p class="h4 mt-3">Три основных режима работы точки доступа:</p>
        <div class="border rounded p-2 overflow-auto" style="font-size:1.2rem;">
            <p>1. Режим «точка доступа»
            В новом оборудовании режим «точка доступа» установлен по умолчанию. В этом режиме Вы подключаетесь со своего компьютера, оснащенного Wi-Fi адаптером, к беспроводной сети Вашей точки доступа. В большинстве случаев для работы в этом режиме специфические настройки не требуются.
            <br>
            2. Режим «мост»
            В этом режиме «мост» точка доступа объединяет физически удаленные сегменты сети в одно целое. Используется при построении «линков» или, другими словами, обеспечения связи между отдаленными объектами.
            <br>
            3. Режим «репитер» (ретранслятор)
            В данном режиме точка доступа работает как приемо-передатчик или «повторитель». Она принимает слабый сигнал от другой точки доступа и, усиливая его, передает на этой же частоте дальше до необходимого адресата.
            </p>
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
        left:'-50%',
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