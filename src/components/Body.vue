<template>
    <div>
        <nav>
            <NavBar :buttons="buttons"/>
        </nav>
        <div>
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
            buttons: [
                "Home",
                "About",
                "Site",
                "More"
            ]
        }
    }
}
</script>