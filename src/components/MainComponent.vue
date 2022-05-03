<template>
    <main id="site_main">
        <div class="container_top">
            <p> --> Content goes Here</p>
        </div>
        <div class="container_bottom">
            <div class="dc_actions">
                <div class="dc_action">
                    <img src="@/assets/img/buy-comics-digital-comics.png" alt="">
                    <p>Digital Comics</p>
                </div>
                <div class="dc_action">
                    <img src="@/assets/img/buy-comics-merchandise.png" alt="">
                    <p>DC Merchandise</p>
                </div>
                <div class="dc_action">
                    <img src="@/assets/img/buy-comics-subscriptions.png" alt="">
                    <p>Subscription</p>
                </div>
                <div class="dc_action">
                    <img src="@/assets/img/buy-comics-shop-locator.png" alt="">
                    <p>Comic Shop Locator</p>
                </div>
                <div class="dc_action">
                    <img src="@/assets/img/buy-dc-power-visa.svg" alt="">
                    <p>DC Power Visa</p>
                </div>
            </div>
        </div>
    </main>
</template>

<script>

</script>

<style lang="scss" scoped>
    main {
     width: 100%;
    }

    .container_top {
        height: 50%;
        background-image: url("@/assets/img/jumbotron.jpg");
        background-size: cover;
        background-repeat: no-repeat;
        padding: 3rem 10rem;
        p {
            color: white;
            font-size: 25px;
            background-color: rgba(0, 0, 0, 0.473)
        }
    }

    .container_bottom {
        height: 50%;
        background-color: rgb(58, 116, 223);
        .dc_actions {
            padding: 3rem 0;
            margin: auto;
            display: flex;
            justify-content: center;
            align-items: center;
            column-gap: 2rem;
            .dc_action {
                color: white;
                display: flex;
                align-items: center;
                column-gap: 0.6rem;
                img {
                    width: 35px;
                }
            }
        }
    }
</style>