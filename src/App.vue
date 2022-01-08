<template>
  <div>
  <Header/>
  <firstComponent/>
  <lifeCycle/>
  <pessoa/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import firstComponent from './components/firstComponent.vue'
import lifeCycle from './components/lifeCycle.vue'
import pessoa from './components/pessoa.vue'

export default{
  name: 'App',
  components:{
    Header,
    firstComponent,
    lifeCycle,
    pessoa
  }
}
</script>

<style>
body{
  background-color: #333;
  color: #FFF;
}

a{
  color: red;
}

.portfolio{
  background-color: #000;
}
</style>