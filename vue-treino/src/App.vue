<template>
    <TheHeader :propsChild="posts"></TheHeader>
    <div v-bind:class="container">
        <h1>{{ title }}</h1>
    </div>
</template>

<script>

import TheHeader from './components/TheHeader.vue';
    
    

    export default {
        name: 'App',
        components: {
            TheHeader,
        },
        data() {
            return {
                title: 'Hello, World',

                container: 'container',

                posts: [
                    {id: 1, valorDinamico: "Treinando componentes 1"},
                    {id: 2, valorDinamico: "Treinando componentes 2"},
                    {id: 3, valorDinamico: "Treinando componentes 3 "},
                    {id: 4, valorDinamico: "Treinando componentes 4 "},
                ],
            }
        },
    }
    
</script>

<style>
    
</style>