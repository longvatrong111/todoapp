<template>
    <div id="app">
        <list v-bind:tasks="tasks"></list>
    </div>
</template>

<script>
    import list from './components/List';

    export default {
        name: 'app',
        components: {list},
        data() {
            return {
                tasks: [{
                    title: 'Ring of Heal',
                    done: true
                }, {
                    title: 'Power Treat',
                    done: true
                }, {
                    title: 'Battle Fury',
                    done: false
                }]
            }
        }
    }
</script>

<style>
    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
</style>
