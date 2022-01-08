<template>
<h1>Meu nome é: {{nome}}</h1>

</template>

<script>
export default{
    name: 'lifeCycle',
    data(){
        return{
            nome: 'Ainda não sei'
            }
        },
        created(){
            setTimeout(() =>
            this.nome = "Arthur"
            , 1000)

            this.lifeCycle()
        },
        mounted(){
            setTimeout(() =>
            this.nome = "Isvi"
            , 2000)

            this.lifeCycle()
        }, 
        methods:{
            lifeCycle(){
                console.log("Executou")
            }
        
        }

    }

</script>