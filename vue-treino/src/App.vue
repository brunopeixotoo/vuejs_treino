<template>
    <TheHeader v-if="showHeader"></TheHeader>
    <div>   
        <h1>Nome</h1>
        {{ name }}
       
        <button
            @click="openAndClosed()"
        >
            Toogle
        </button>
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
                name: "Lucas",
                showHeader: true,
            }
        },
        //HOOKS
        // beforeCreate() {
        //     console.log('beforeCreate');
        //     console.log('Estado:', this.name);
        //     console.log('DOM:', this.$el);
        // },
        // created() {
        //     console.log('create');
        //     console.log('Estado:', this.name);
        //     console.log('DOM:', this.$el);
        // },
        // beforeMount() {
        //     console.log('beforeMount');
        //     console.log('Estado:', this.name);
        //     console.log('DOM:', this.$el);
        // },
        // mounted() {
        //     console.log('mounted');
        //     console.log('Estado:', this.name);
        //     console.log('DOM:', this.$el);
        // },


        watch: {

        },
        computed: {

        },
        methods: {
            openAndClosed() {
                this.showHeader = !this.showHeader;
            }
        },
    }
    
</script>

<style>
    
</style>