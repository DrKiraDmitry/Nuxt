<template>
    <div class="index">
        <div class="synergy row no-gutters">
            <div class="twoFace col-8 col-xl-4 offset-1">
                <img src="~/assets/img/twoFaceD.png" alt="">
                <img src="~/assets/img/twoFace.png" alt="">
            </div>
            <div class="col-xl-4 col-10 offset-xl-2 offset-1">
                <h3>Синергия</h3>
                <p>Во мне сочетается много всего, мне очень нравится искусство, точные науки и психология.</p>
                <p>И здесь я постраюсь отобразить, то что порождает эта Синергия</p>
            </div>
        </div>
        <div class="DeusEx row no-gutters">
            <animation class="col-xl-5 col-12" />
            <div class="col-xl-4 col-10 offset-xl-2 offset-1">
                <h3>Начало положенно</h3>
                <p>Изначально было желание поиграться с векторной анимацией, хотелось разобраться как это делать.</p>
                <p>В плейлисте заиграл OST Deus Ex: Human Revolution, и мне вспомнилась аниация на начальном экране, как портрет Адама, разбиралася и собирался по кусочкам.</p>
                <p>Тогда стало ясно, какую аниацию я хочу.</p>
                <p>Пришлось заморочится, чтоб каждый элемент, улетал по отдельности</p>
            </div>             
        </div>
        <div class="row no-gutters index__psychology">
            <div class="index__psychology__table col-10 offset-1">
                <div class="index__psychology__toggle">
                    <a @click="id = user.id" v-for="(user, index) in users" :key="index" :class="{active: id == user.id}">
                        {{user.head}}
                    </a>
                </div>
                <div class="index__psychology__body" v-for="(user, index) in users" :key="index" v-show="id == user.id">
                    <div class="perspective">
                        <img :src="user.img" alt="">
                    </div>
                    <div class="index__psychology__body__text">
                        <h3>{{user.title}}</h3>
                        <p v-for="(index, data) in user.data" :key="data">{{index.p}}</p>
                    </div>                  
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import animation from '~/components/animation.vue'
export default {
    components:{
        animation,
    },
    data() {
        return {
            id:'1',
            users:[
                {
                id: 1,
                head:"Оглавление",
                title: "Игры в которые играю люди",
                img: "/_nuxt/assets/img/psi31.png",
                data: [{"p":"Ответ на то, как и почему это происходит, дает трансакционный или трансактный анализ – психологическая модель, разработанная американским психологом Эриком Берном. Он изложил ее в своих книгах о психологии взаимоотношений: «Игры, в которые играют люди» и «Люди, которые играют в игры»"},{"p":5}]
                },
                {
                id: 2,
                head:"Я-ребенок",
                title: "Я-ребенок",
                img: "/_nuxt/assets/img/child.png",
                data: [{"p":1},{"p":3},{"p":5}]
                },
                {
                id: 3,
                head:"Я-родитель",
                title: "Я-родитель",
                img: "/_nuxt/assets/img/psi31.png",
                data: [{"p":1},{"p":3},{"p":5}]
                },
                {
                id: 4,
                head:"Я-взрослый",
                title: "Я-взрослый",
                img: "/_nuxt/assets/img/psi31.png",
                data: [{"p":1},{"p":3},{"p":5}]
                },
            ]
        }
    },
    methods:{
        function (){
            
        }
    },
    mounted(){

    }
}
</script>
