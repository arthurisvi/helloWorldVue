<template>
<div>
    <h1>
    Olá, Vue!
    </h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <MultipleEvents/>
</div>
</template>

<script>
import MultipleEvents from './MultipleEvents.vue'

export default{
  name: 'firstComponent',
  components:{
    MultipleEvents
  },
  data(){
      return{
          nome: "Arthur",
          profissao: "Progamador"
          }
  }
  }
</script>