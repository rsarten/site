<template>
    <div>
        <nav>
            <NavBar :buttons="buttons" v-on:setBody="updateBody($event)" />
        </nav>
        <div>
            <h2>The body is now displaying {{ title }}</h2>
            <Content/>
        </div>
    </div>
</template>

<script>
import NavBar from './NavBar'
import Content from './Content'

export default {
    name: 'Body',
    components: {
        'NavBar': NavBar,
        'Content': Content
    },
    data() {
        return {
            title: "HomeHome",
            buttons: [
                "Home",
                "About",
                "Site",
                "More"
            ]
        }
    },
    methods: {
        updateBody: function(page) {
            this.title = page
        }
    }
}
</script>