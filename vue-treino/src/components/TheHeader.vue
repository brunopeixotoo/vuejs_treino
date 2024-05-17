<template>
    <div :class="theheader">
       <h1>{{ title }}</h1>
    </div>
</template>

<script>
  
    export default {
        name: 'TheHeader',
        data() {
            return {
                title: "The Header",



                theheader: "header",
            }
        },
        beforeUnmount() {
            console.log('beforeUnmount');
            
        },
        unmounted() {
            console.log('unmounted');
           
        },

    }
    
</script>

<style>
    .header {
        background-color: rgb(0, 102, 255);
    }
</style>