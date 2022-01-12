<template>
    <div>
        <button @click="$emit('changePicture')">Trocar imagem de perfril</button>
    </div>
</template>

<script>
export default{
    name: 'ChangePicture',
    emits: 'changePicture'
}
</script>