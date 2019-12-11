<template>
  <div class="no-gutters">
    <header class="col-10 offset-1 row no-gutters justify-content-between">
        <div class="logo col-4 col-xl-1">
          <nuxt-link :to="{name: 'index'}">MIKIRI</nuxt-link>
        </div>
        <div class="menu__link col-2 col-xl-6">
          <svg id="menu__bar" @click="menu = !menu" width="23" height="23"  viewBox="0 0 23 23" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path :class="{bar1: menu}" d="M0 0.5H23" stroke="#FFE0E0"/>
              <path :class="{bar2: menu}" d="M0 11.246H23" stroke="#FFE0E0"/>
              <path :class="{bar3: menu}" d="M0 22H23" stroke="#FFE0E0"/>
          </svg>            
          <div id="menu__mobile" :class="{menu__mobileon: menu}" class="menu">
              <nuxt-link :to="{name: 'index'}">Главная</nuxt-link>
              <nuxt-link :to="{name: 'second'}">Анимация и Js</nuxt-link>
              <a>Векторная Графика</a>
              <a href="#">Верстка и Api</a>
          </div>
        </div>
    </header>
    <nuxt />
    <footer class="row no-gutters justify-content-between">
          <p class="col-1 offset-1">Mikiri@2017-2019</p>
          <div class="col-1">
            <i class="fab fa-github"></i>
            <i class="fab fa-instagram"></i>
          </div>
    </footer>
  </div>
</template>
<script>
export default {
  data(){
    return{
      menu:false,
    }
  }
}
</script>