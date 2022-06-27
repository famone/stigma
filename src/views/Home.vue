<template>
  <div>
    <Main /> 
    <About />
    <Serv />
    <Advant />
    <Tech />
    <Faq />
    <Cont />
    <Copyright />
  </div>
</template>

<script>
import Main from '../components/Main.vue'
import About from '../components/About.vue'
import Serv from '../components/Serv.vue'
import Advant from '../components/Advant.vue'
import Tech from '../components/Tech.vue'
import Faq from '../components/Faq.vue'
import Cont from '../components/Cont.vue'
import Copyright from '../components/Copyright.vue'

export default {
  components: {Main, About, Serv, Advant, Tech, Faq, Cont, Copyright}
}
</script>
