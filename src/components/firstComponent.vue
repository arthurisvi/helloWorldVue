<template>
<div>
    <h1>
    Olá, Vue!
    </h1>
    <p>Meu nome é {{ nome }} e trabalho como {{ profissao }}</p>
    <MultipleEvents/>
    <Reuse/>
    <Reuse/>
    <Reuse/>
</div>
</template>

<script>
import MultipleEvents from './MultipleEvents.vue'
import Reuse from './Reuse.vue'

export default{
  name: 'firstComponent',
  components:{
    MultipleEvents,
    Reuse
  },
  data(){
      return{
          nome: "Arthur",
          profissao: "Progamador"
          }
  }
  }
</script>