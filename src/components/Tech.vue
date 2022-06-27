<template>
    <section id="tech">
        <div class="container">
            <div class="row">
                <div class="col-lg-4" style="position:relative;">
                    <img src="../assets/img/tech.png" class="tech-bg wow fadeInLeft">
                </div>
                <div class="col-lg-7 offset-lg-1">
                    <div class="overhidden mb-6">
                        <p class="mb-0 wow slideInUp gray-txt">Дело техники</p>
                    </div>
                    <div class="overhidden mb-40">
                        <h2 class="mb-0  wow slideInUp">Устройства мониторинга</h2>
                    </div>
                    <p class="simple-txt mb-40">Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum esse dolor iste sapiente ullam ab debitis odit neque repellat repellendus, accusamus sed eius eos magni distinctio voluptatum odio eligendi facilis doloribus! Voluptate aliquid voluptas facilis quaerat. </p>

                    <div class="row">
                        <div class="col-lg-6" v-for="(item, id) in tech" :key="id">
                            <div class="tech-icon">
                                <img :src="item.img" alt="">
                                <h4 class="mb-6">{{item.name}}</h4>
                                <p class="simple-txt">Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum esse door.</p>
                            </div>
                        </div>
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
            tech: [
                {   
                    img: require('../assets/img/t1.png'),
                    name: 'Статус блокировки'
                },
                {   
                    img: require('../assets/img/t2.png'),
                    name: 'Зарядка более 30 дней'
                },
                {   
                    img: require('../assets/img/t3.png'),
                    name: 'Шифрование данных'
                },
                {   
                    img: require('../assets/img/t4.png'),
                    name: 'Прочный корпус'
                },
            ]
        }
    }
}
</script>