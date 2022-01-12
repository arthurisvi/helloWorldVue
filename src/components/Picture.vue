<template>
    <!-- mesma coisa de usar o -v-bind:-->
    <div>
    <img :src="avatar" :alt="descricao">
    <!--<Reuse/> -->
    <ChangePicture @change-picture="changePicture"/>

    </div>
</template>

<script>
// import Reuse from './Reuse.vue'
import ChangePicture from './ChangePicture.vue'

export default{
    name: 'Picture',
    components:{
        // Reuse,
        ChangePicture
    },
    data(){
        return{
            //por padrão acessa a pasta public
            avatar: "/img/avatar.png",
            descricao: "Arthur Isvi"
        }
    }, methods:{
        changePicture(){
            this.avatar = "/img/avatar2.png"
        }
    }
}

</script>