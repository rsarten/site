<template>
    <div class="nav-bar">
        <p>list of navigation buttons</p>
        <ol>
            <div v-for="button in buttons" v-bind:key="button">
            <nav-button :name=button />
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
    props: ['buttons']
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