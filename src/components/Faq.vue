<template>
    <section id="faq">
        <div class="container">
            <div class="row trial wow fadeInUp">
                <div class="col-lg-10 offset-lg-1">
                    <div class="trial-box">
                        <div class="row">
                            <div class="col-lg-10">
                                <p class="gray-txt">Trial</p>
                                <h2>Бесплатный пробный период – <span class="blue">14 дней</span></h2>
                                <p class="white-txt">Познакомьтесь с нашей системой абсолютно бесплатно и убедитесь в её удобстве для вас за две недели доступа ко всем её возможностям.</p>
                                <button class="simple-btn">
                                    Оформить заявку
                                    <span class="mdi mdi-arrow-right"></span>
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="col-lg-10 offset-lg-1">
                    <div class="overhidden mb-6">
                        <p class="mb-0 wow slideInUp gray-txt">FAQ</p>
                    </div>
                    <div class="overhidden mb-40">
                        <h2 class="mb-0  wow slideInUp">Вопросы и ответы</h2>
                    </div>
                    <div class="row">
                        <div class="col-lg-6">
                            <div class="acc" v-for="(item, id) in faqs" :key="id"
                            :class="{activeAc : item.active}" @click="item.active = !item.active">
                                <div class="acc-head">
                                    <h4>{{item.name}}</h4>
                                    <span class="mdi mdi-chevron-down"></span>
                                </div>
                                <div class="acc-body">
                                    <p class="simple-txt">
                                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum esse dolor iste sapiente ullam ab debitis odit neque repellat repellendus, accusamus sed eius eos magni distinctio voluptatum odio eligendi facilis doloribus! Voluptate aliquid voluptas facilis quaerat. 
                                    </p>
                                </div>
                            </div>
                        </div>
                        <div class="col-lg-6">
                            <div class="acc" v-for="(item, id) in faqs2" :key="id"
                            :class="{activeAc : item.active}" @click="item.active = !item.active">
                                <div class="acc-head">
                                    <h4>{{item.name}}</h4>
                                    <span class="mdi mdi-chevron-down"></span>
                                </div>
                                <div class="acc-body">
                                    <p class="simple-txt">
                                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum esse dolor iste sapiente ullam ab debitis odit neque repellat repellendus, accusamus sed eius eos magni distinctio voluptatum odio eligendi facilis doloribus! Voluptate aliquid voluptas facilis quaerat. 
                                    </p>
                                </div>
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
            faqs: [
                {
                    name: 'Контроль на складе',
                    active: true
                },
                {
                    name: 'Как долго работает пломба без зарядки?',
                    active: false
                },
                {
                    name: 'Контроль на складе',
                    active: false
                },
            ],
            faqs2: [
                {
                    name: 'Контроль на складе',
                    active: false
                },
                {
                    name: 'Как долго работает пломба без зарядки?',
                    active: false
                },
                {
                    name: 'Контроль на складе',
                    active: false
                },
            ]
        }
    }
}
</script>