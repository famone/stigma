<template>
    <section id="cont">
        <div class="container">
            <div class="row">
                <div class="col-lg-3" v-for="(item, index) in contacts" :key="index">
                    <div class="serv-box">
                        <img :src="item.img" alt="">
                        <p class="simple-txt">{{item.txt}}</p>
                        <h4 v-html="item.name"></h4>
                    </div>
                </div>
                <div class="col-lg-12 text-center">
                    <button class="blue-btn" style="margin:0 auto;">
                        Посмотреть на карте
                        <span class="mdi mdi-arrow-right"></span>
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data(){
        return{
            contacts: [
                {
                    img: require('../assets/img/c1.png'),
                    txt: 'Адрес',
                    name: 'Республика Беларусь <br> г. Минск, Богдановича 7'
                },
                {
                    img: require('../assets/img/c2.png'),
                    txt: 'Телефон',
                    name: '+375 (29) 609-08-09 <br><br>'
                },
                {
                    img: require('../assets/img/c3.png'),
                    txt: 'E-mail',
                    name: 'office@realservice.site <br><br>'
                },
                {
                    img: require('../assets/img/c4.png'),
                    txt: 'Юр. информация',
                    name: 'УНП: 193155389 <br> ООО Настоящий сервис'
                },
            ]
        }
    }
}
</script>