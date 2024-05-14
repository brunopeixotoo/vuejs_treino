<template>
    <div v-bind:class="container">
        <p>{{ valorProp }}</p>
    </div>
</template>

<script>
  
    export default {
        name: 'TheHeader',
        props: {
            valorProp: String,
        },
        data() {
            return {
                title: 'Treinando',
                container: 'container',
            }
        },
    }
    
</script>

<style>
    .container {
        margin: 20px auto 20px auto;
        display: flex;
        align-items: center;
        justify-content: center;
    }
</style>