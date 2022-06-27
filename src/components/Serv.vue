<template>
    <section id="serv">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="overhidden mb-6">
                        <p class="mb-0 wow slideInUp gray-txt">Мы предоставляем</p>
                    </div>
                    <div class="overhidden mb-40">
                        <h2 class="mb-0  wow slideInUp">Наша специализация</h2>
                    </div>
                </div>
                <div class="col-lg-3" v-for="(item, index) in services" :key="index">
                    <div class="serv-box">
                        <img :src="item.img" alt="">
                        <h4 v-html="item.name"></h4>
                        <p class="simple-txt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum esse door.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    data(){
        return{
            services: [
                {
                    img: require('../assets/img/s1.png'),
                    name: 'Онлайн трекинг транспорта'
                },
                {
                    img: require('../assets/img/s2.png'),
                    name: 'Контроль на <br> складе'
                },
                {
                    img: require('../assets/img/s3.png'),
                    name: 'Отслеживание статуса отправки'
                },
                {
                    img: require('../assets/img/s4.png'),
                    name: 'Помощь в таможенном оформлении'
                },
            ]
        }
    }
}
</script>