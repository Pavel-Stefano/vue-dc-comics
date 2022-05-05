<template>
    <div class="top-footer">
            <div class="container">
                <ul>
                    <li class="icon-footer" v-for="(box, index) in cardFooter" :key="index">
                        <img :src="box.src" alt="" :key="index">
                        <p>{{box.titolo}}</p>
                    </li>
                </ul>
                
            </div>
            
        </div>
</template>

<script>
export default {
    name: 'TopFooter',
    data(){
        return {
            cardFooter:[
                {
                src: require("../assets/images/buy-comics-digital-comics.png"),
                titolo: "Digital comics",
                },
                {
                src: require("../assets/images/buy-comics-merchandise.png"),
                titolo: "Dc merchandise",
                },
                {
                src: require("../assets/images/buy-comics-subscriptions.png"),
                titolo: "Subscription",
                },
                {
                src: require("../assets/images/buy-comics-shop-locator.png"),
                titolo: "Comic shop locator",
                },
                {
                src: require("../assets/images/buy-dc-power-visa.svg"),
                titolo: "Dc power visa",
                },
            ] 
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.top-footer {
    background-color: $bgAzzurro;
    color: $testoBianco;
    padding: 40px 0;
}

.container {
    justify-content: space-around;
}

ul {
    width: 100%;
}

.icon-footer {
    display: flex;
    justify-content: space-around;
    align-items: center;
    gap: 7px;
    margin: 0 25px;
    z-index: 100;
}

.icon-footer img {
    width: 50px;
}

</style>