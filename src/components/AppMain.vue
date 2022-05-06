<template>
    <main>
        <jumbo-main />
        <grid-main />
        
    </main>
</template>

<script>

import GridMain from '../components/GridMain.vue'
import JumboMain from '../components/JumboMain.vue'
export default {
    components: {
        JumboMain,
        GridMain,
    },
    name: 'AppMain',
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
main {
    background-color: $bgNero;
    color: $testoBianco;
    padding: 25px 0;
}

.jumbo-main {
    height: 400px;
    background-image: url('../assets/images/jumbotron.jpg');
    background-size: cover;
    background-position: top center;
}

</style>