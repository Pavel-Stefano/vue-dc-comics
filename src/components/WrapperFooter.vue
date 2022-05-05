<template>
    <div class="wrapper-footer">
        <div class="container wrapper">
            <div class="right">
                <div class="list">
                    <h3>DC Comics</h3>
                    <ul>
                        <li v-for="(link, index) in Comics" :key="index">{{ link }}</li>
                    </ul>
                    <h3>Shop</h3>
                    <ul>
                        <li v-for="(link, index) in Shop" :key="index">{{ link }}</li>
                    </ul>
                </div>

                <div class="list">
                    <h3>DC</h3>
                    <ul>
                        <li v-for="(link, index) in DC" :key="index">{{ link }}</li>
                    </ul>
                </div>

                <div class="list">
                    <h3>Sites</h3>
                    <ul>
                        <li v-for="(link, index) in Sites" :key="index">{{ link }}</li>
                    </ul>
                </div>
            </div>
            

            <div class="wrapper-image">
                <img src="../assets/images/dc-logo-bg.png" alt="">
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: 'WrapperFooter',
    data(){
        return {
            Comics: [
                "Characters",
                "Comics",
                "Movies",
                "Tv",
                "Games",
                "Videos",
                "News",
            ],
            Shop: [
                "Shop DC",
                "Shop DC Collectibles"
            ],
            DC: [
                "Terms Of Use",
                "Privacy policy(New)",
                "Ad Choices",
                "Advertising",
                "Jobs",
                "Subscriptions",
                "Talent Workshop",
                "CPSC Certificates",
                "Ratings",
                "Shop Help",
                "Contact Us",
            ],
            Sites: [
                "DC",
                "MAD Magazine",
                "DC Kids",
                "DC Universe",
                "DC Power Visa",
            ],
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';

.wrapper-footer {
    color: $testoBianco;
    .container.wrapper {
        padding: 0;
        align-items: flex-start;
        .right {
            padding: 70px 0;
            display: flex;
            gap: 50px;
            h3 {
            text-transform: uppercase;
            font-size: 20px;
            }
            ul {
                display: flex;
                flex-direction: column;
                padding: 15px 0;
                li {
                    margin: 3px 0;
                    color: grey;
                    text-transform: capitalize;
                }
            }
        }
    } 
}

.wrapper-image {
    width: 40%;
}

.wrapper-image img{
    position: relative;
    top: -105px;
    width: 110%;
}


</style>