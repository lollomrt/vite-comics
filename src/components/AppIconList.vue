<script>
export default {

}
</script>

<template lang="">
    <div class="blue-section">
        <div class="container">
        <div class="card">
            <img src="../assets/Images/buy-comics-digital-comics.png" alt="">
            <span class="icon-text">digital comics</span>
        </div>
        <div class="card">
            <img src="../assets/Images/buy-comics-merchandise.png" alt="">
            <span class="icon-text">dc merchandise</span>
        </div>
        <div class="card">
            <img src="../assets/Images/buy-comics-subscriptions.png" alt="">
            <span class="icon-text">subscription</span>
        </div>
        <div class="card">
            <img src="../assets/Images/buy-comics-shop-locator.png" alt="">
            <span class="icon-text">comic shop locator</span>
        </div>
        <div class="card">
            <img src="../assets/Images/buy-dc-power-visa.svg" alt="">
            <span class="icon-text">dc power visa</span>
        </div>
    </div>
    </div>
</template>

<style lang="scss">
@use '../styles/partials/variables.scss' as *;
@use '../styles/partials/mixins.scss' as *;

.blue-section {
    background-color: $primary;
    @include flex-center;

    .container {
        width: 1200px;
        @include flex-between;
        padding: 3rem 0;

        .card {
            width: calc(100% / 5);
            display: flex;
            align-items: center;
            gap: 1rem;

            &:nth-child(4) img {
                width: 30px;
            }

            img {
                width: 40px;
            }

            .icon-text {
                text-transform: uppercase;
                color: #fff;
                font-size: 0.9rem;
            }
        }
    }
}
</style>