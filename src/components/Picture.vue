<template>
    <!-- mesma coisa de usar o -v-bind:-->
    <img :src="avatar" :alt="descricao">
</template>

<script>
export default{
    name: 'Picture',
    data(){
        return{
            //por padrão acessa a pasta public
            avatar: "/img/avatar.png",
            descricao: "Arthur Isvi"
        }
    }
}

</script>