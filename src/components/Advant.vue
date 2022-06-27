<template>
    <section id="advant">
        <div class="mock"></div>
        <div class="container">
            <div class="row">
                <div class="col-lg-4">
                    <p class="gray-txt">Почему мы?</p>
                    <h2>Наши преимущества</h2>
                    <div class="advant-item" :class="{'mb-0' : id+1 == advantages.length}" v-for="(item, id) in advantages" :key="id"> 
                        <p class="gray-txt">0{{id+1}}</p>
                        <div>
                            <h4 class="mb-6">{{item.name}}</h4>
                            <p class="simple-txt">
                                Lorem ipsum dolor sit amet consectetur adipisicing elit. Illum esse door.
                            </p>
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
            advantages: [
                {
                    name: 'Поиск и аналитика'
                },
                {
                    name: 'Удобное ПО'
                },
                {
                    name: 'Интеграции и разработка'
                },
                {
                    name: 'Поддержка'
                },
            ]
        }
    }
}
</script>