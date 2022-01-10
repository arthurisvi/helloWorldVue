<template>
    <!-- mesma coisa de usar o -v-bind:-->
    <div>
    <img :src="avatar" :alt="descricao">
    <Reuse/>

    </div>
</template>

<script>
import Reuse from './Reuse.vue'

export default{
    name: 'Picture',
    components:{
        Reuse
    },
    data(){
        return{
            //por padrão acessa a pasta public
            avatar: "/img/avatar.png",
            descricao: "Arthur Isvi"
        }
    }
}

</script>