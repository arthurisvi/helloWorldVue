<template>
<div>
    <p v-if="isWorking">Estou trabalhando no momento</p>
    <p v-else>No momento estou a procura de trabalho.</p>
    <p>Utilizo as seguintes tecnologias: </p>
    <ul>
        <li>JavaScript</li>
        <li>Java</li>
        <li>Python</li>
    </ul>
    <div>
        <button @click="showEmail">{{ textButton }}</button>
    </div>

    <!-- v-show é um boolean, só utiliza para fazer algo qnd for true-->
    <p v-show="showTextEmail">Mande uma mensagem para {{ email }}</p>
    <!-- v-bind interpreta o link como um dado dinâmico-->
    <p class="portfolio">Para acessar meu portfólio <a v-bind:href="myLink" target="blank">basta clicar aqui</a></p>
    <Picture/>
    <div>
    <p>Testando se importou componente</p>
    </div>
    </div>
</template>

<script>
import Picture from './Picture.vue'
export default{
    name: 'info',
    components:{
        Picture
    },
    data(){
        return {
            isWorking: false,
            showTextEmail: false,
            email: 'spfcarthur1@gmail.com',
            myLink: 'https://google.com',
            textButton: 'Mostrar e-mail'
        }
    },methods:{
        showEmail(){
            this.showTextEmail = !this.showTextEmail
            if(!this.showTextEmail){
                this.textButton = "Mostrar e-mail"
            }else{
                this.textButton = "Esconder e-mail"
            }
        }


    }



}
</script>