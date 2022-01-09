<template>
    <div>
    <form action = "" @submit="sendForm($event)">
        <div>
            <input type = "text" v-model="name">
    <!--<InputText/> -->
        </div>
        <div>
            <input type = "text" v-model="email">
    <!--<InputText/> -->
        </div>
    <div>
    <Submit/>
    </div>
    </form>
    <p>Conteúdo</p>
    <p>Conteúdo</p>    
    <p>Conteúdo</p>        
    </div>
</template>

<script>
import Submit from './form/Submit.vue'
import InputText from './form/InputText.vue'

export default{
    name: 'Form',
    components:{
        InputText,
        Submit
    }, 
    data(){
        return{
            name: "",
            email: ""
        }
    },
    methods:{
        sendForm(e){
            e.preventDefault();
            const name = this.name;
            const email = this.email;
            console.log("Formulario enviado!")
            console.log("O nome é: " + name)
            console.log("O email é: " + email)

            //Ajax  - requisicao async com o servidor - Inserir no banco
        }
    }
}

</script>

<style scoped>
    p{
        margin: 150px;
    }
</style>