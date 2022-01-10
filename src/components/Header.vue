<template>
<ul>
    <li><a href="#">Home</a></li>
    <li><a href="#">Projetos</a></li>
    <li><a href="#">Contato</a></li>
    <li v-if="isLogged"><a href="#">Meu Perfil</a></li>
</ul>
</template>

<script>
export default{
    name:'Header',
    props: ["isLogged"]
}
</script>

<style scoped>
    ul{
        list-style: none;
        display: flex;
        background: #999
    }

    li{
        margin-right: 10px;
    }

    a{
        color: #DDD;
        text-decoration: none;
        transition: .5s;
    }

    a:hover{
        color: red;
    }

</style>