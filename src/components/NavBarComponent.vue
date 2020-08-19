<template>
    <div class="nav-bar">
        <p>list of navigation buttons</p>
        <ol>
            <li v-for="label in labels" v-bind:key="label">
            {{ label.display }}
            </li>
        </ol>
    </div>
</template>

<script>
export default {
    name: 'NavBarComponent',
    data() {
        return {
            labels: [
                {'label': 'Home', 'display': 'Home'},
                {'label': 'Graph', 'display': 'Graph'},
                {'label': 'About', 'display': 'About me'}
            ]
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