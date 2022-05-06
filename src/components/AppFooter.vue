<template>
    <footer>
        
        <top-footer />

        <wrapper-footer />

        <down-footer />

    </footer>
</template>

<script>
import TopFooter from '../components/TopFooter.vue'
import WrapperFooter from '../components/WrapperFooter.vue'
import DownFooter from '../components/DownFooter.vue'



export default {
  components: { 
      TopFooter,
      WrapperFooter,
      DownFooter,
      },
    name: 'AppFooter',
   
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.wrapper-footer {
    height: 360px;
    background-image: url('../assets/images/footer-bg.jpg');
    background-size: cover;
    overflow: hidden;
}

</style>