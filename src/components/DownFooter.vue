<template>
    <div class="down-footer">
        <div class="container">
            <div class="btn">
                <a href="#"> Sign-up Now!</a>
            </div>
            <div class="socials">
                <h2>Follow Us</h2>
                <div><img src="../assets/images/footer-facebook.png" alt=""></div>
                <div><img src="../assets/images/footer-twitter.png" alt=""></div>
                <div><img src="../assets/images/footer-youtube.png" alt=""></div>
                <div><img src="../assets/images/footer-pinterest.png" alt=""></div>
                <div><img src="../assets/images/footer-periscope.png" alt=""></div>
            </div>
            
        </div>
    </div>
</template>

<script>
export default {
    name: 'DownFooter',
}
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
.down-footer {
    background: $bgGrigio;
    height: 90px;
    .container {
        height: 100%;
        .socials {
            display: flex;
            align-items: center;
            gap: 20px;
            h2 {
                color: $bgAzzurro;
                text-transform: uppercase;
            }
        }
    }
}

.btn a {
    text-decoration: none;
    padding: 11px 8px;
    border: 2px solid $bgAzzurro;
    color: $testoBianco;
}
</style>