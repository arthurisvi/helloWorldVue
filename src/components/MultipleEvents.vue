<template>
<div>
    <button @click="first(txt1, $event), second(txt2, $event)">Ativar mútiplos eventos</button>
    <p>{{ multipleEvents}}</p>
</div>

</template>

<script>
    export default{
        name: "MultipleEvents",
        data(){
            return{
                multipleEvents: "",
                txt1: "Primeiro evento!",
                txt2: "Segundo evento!"
            }
        },methods:{
            first(txt, e){
               this.multipleEvents = txt
            },
            second (txt, e){
                setTimeout(()=>this.multipleEvents = txt, 500)
            }

        }
    }

</script>

<style scoped>
    div{
        margin: 100px;
    }

</style>