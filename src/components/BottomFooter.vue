<template>
    <section>
        <div class="container">
            <div>
                <a href="#">sign-up now!</a>
            </div>
            <div>
                <span>follow us</span>
                <img src="/img/footer-facebook.png" alt="">
                <img src="/img/footer-twitter.png" alt="">
                <img src="/img/footer-youtube.png" alt="">
                <img src="/img/footer-pinterest.png" alt="">
                <img src="/img/footer-periscope.png" alt="">
            </div>
        </div>
    </section>
</template>

<script>
    export default {
        name: 'BottomFooter',
    }
</script>

<style lang="scss" scoped>
 *
    section {
        background-color: #303030;
        padding: 30px 0;
        .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 20px;

            a {
            text-decoration: none;
            text-transform: uppercase;
            color: white;
            border: 2px solid #0282F9;
            padding: 10px 20px;
            }

            span {
                color: #0282F9;
                text-transform: uppercase;
                font-weight: 700;
                padding: 0 20px;
            }
            img {
                padding: 0 10px;
            }
        }
        
    }

</style>