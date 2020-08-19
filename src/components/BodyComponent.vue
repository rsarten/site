<template>
    <div>
        <nav>
            <NavBarComponent/>
        </nav>
        <div>
            <ContentComponent/>
        </div>
    </div>
</template>

<script>
import NavBarComponent from './NavBarComponent'
import ContentComponent from './ContentComponent'

export default {
    name: 'BodyComponent',
    components: {
        'NavBarComponent': NavBarComponent,
        'ContentComponent': ContentComponent
    }
}
</script>