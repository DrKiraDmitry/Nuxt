<template>
  <div>
    <div class="DeusEx">
          <animation/>
          <div>
              <h1>Добро пожаловать в компанию MIKIRI</h1>
              <a href="#about">Предложить работу</a>
          </div>             
      </div>
      <div id="about" class="AboutUs">
        <div class="logo">
            <p class="outside">У</p>
            <h2 class="logo__text">Наши услуги</h2>
        </div>
        <div class="row no-gutters">
          <div class="col-10 offset-1 AboutUs__psiblock row no-gutters">
              <div class="block col-12 col-xl-4">
                  <img src="~/assets/img/services1.png" alt="">
                  <div class="block__content">
                      <h1>Векторная Графика</h1>
                      <p>Занимаюсь созданием логотипов и иконок в векторной графике (в формате SVG), их можно использовать как на веб-страницах, так и для размещения на вещах
                      </p>
                      <button>Узнать больше</button>
                  </div>
              </div>
              <div class="block col-12 col-xl-4">
                  <img src="~/assets/img/services2.png" alt="">
                  <div class="block__content">
                      <h1>Анимация и Js</h1>
                      <p>
                          Красивая анимация, это не всегда легко, но она того стоит. Она сделает ваш сайт, живым и запоминающимся. Анимация это не только, выпадающие окна, можно заставить двигаться даже картины
                      </p>
                      <button>Узнать больше</button>
                  </div>
              </div>
              <div class="block col-12 col-xl-4">
                  <img src="~/assets/img/services3.png" alt="">
                  <div class="block__content">
                      <h1>Верстка и Api</h1>
                      <p>
                          "Мне нужен сайт", но сайт это не только страница, ему еще нужна и логика, которая обрабатывается на сервере. Сайт может быть Одностраничный иначе, Лэндинг, а может сложным приложением в которым и чат, и управление заказами. Так что же нужно?
                      </p>    
                      <button>Узнать больше</button>
                  </div>
              </div>
          </div>
        </div>
      </div>
      <div class="row work">
            <div class="twoFace col-4 offset-1">
                <img src="~/assets/img/twoFaceD.png" alt="">
                <img src="~/assets/img/twoFace.png" alt="">
            </div>
            <div class="col-4 offset-1">
                <h3>Синергия</h3>
                <p>Во мне сочетается много всего, мне очень нравится искусство, точные науки и психология.</p>
                <p>И здесь я постраюсь отобразить, то что порождает эта Синергия</p>
            </div>
      </div>
  </div>
</template>

<script>
import animation from '~/components/animation.vue'

export default {
    components:{
        animation
    },
    data() {
        return {
        }
    },
    methods:{
    },
}
</script>
