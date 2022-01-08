<template>
    <div>
    <form action = "">
        <div>
    <InputText/>
        </div>
             <div>
    <InputText/>
        </div>
    <div>
    <Submit/>
    </div>
    </form>    
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
    }
}

</script>