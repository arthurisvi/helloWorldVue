<template>
<div>   
    <h2>Esta é a descrição da pessoa: {{nome}}</h2>
    <info />
    <Form />
</div>
</template>

<script>
import Form from './Form'
import info from './info.vue'
export default{
    name: 'pessoa',
        components: {
            info, 
            Form
        },
    data(){
        return{
            nome: 'Arthur'
            }
        }

    }

</script>