<template>
    <div class="nav-bar">
        <p>{{ title }}</p>
        <ol>
            <div v-for="button in buttons" v-bind:key="button">
                <NavButton :name=button v-on:navClick="updateBody($event)" />
            </div>
        </ol>
    </div>
</template>

<script>
import NavButton from './NavButton.vue'

export default {
    name: 'NavBar',
    components: {
        'NavButton': NavButton
    },
    props: ['buttons'],
    data() {
        return {
            title: "other things:"
        }
    },
    methods: {
        updateBody: function(navname) {
            this.title = navname;
            this.$emit('setBody', navname)
        }
    }
}
</script>

<style scoped>
.nav-bar {
    float: left;
    max-width: 15%;
    margin: 0;
    padding: 1em 1em 1em 0.5em;
    border-style: solid;
    border-width: 5px;
    border-color: brown;
}
</style>