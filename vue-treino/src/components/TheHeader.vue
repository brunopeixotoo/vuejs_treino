<template>
    <div v-bind:class="container">
        <p v-for="post in propsChild" :key="post.id"> Valor: {{ post.valorDinamico }}</p>
    </div>
</template>

<script>
  
    export default {
        name: 'TheHeader',
        props: {
            propsChild: {
                type: Array,
                required: true,
            }
        },
        data() {
            return {
                container: 'container',
            }
        },
    }
    
</script>

<style>
</style>