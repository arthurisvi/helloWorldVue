<template>
  <div>
  <firstComponent/>
  <lifeCycle/>
  <pessoa/>
  </div>
</template>

<script>
import firstComponent from './components/firstComponent.vue'
import lifeCycle from './components/lifeCycle.vue'
import pessoa from './components/pessoa.vue'

export default{
  name: 'App',
  components:{
    firstComponent,
    lifeCycle,
    pessoa
  }
}
</script>