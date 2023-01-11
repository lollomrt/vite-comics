<script>
export default {

}
</script>

<template lang="">
    <footer>
        <div class="sup">
            <div class="container">
                <div class="navigazione">
                    <nav>
                        <h2>DC comics</h2>
                        <ul>
                            <li>Characters</li>
                            <li>Comics</li>
                            <li>Moovies</li>
                            <li>TV</li>
                            <li>Games</li>
                            <li>Videos</li>
                            <li>News</li>
                        </ul>
                    </nav>
                    <nav>
                        <h2>Shop</h2>
                        <ul>
                            <li>Shop DC</li>
                            <li>Shop DC Collectibles</li>
                        </ul>
                    </nav>
                    <nav>
                        <h2>DC</h2>
                        <ul>
                            <li>Therms Of Use</li>
                            <li>Privacy Policy</li>
                            <li>Add Choices</li>
                            <li>Advertising</li>
                            <li>Job</li>
                            <li>Subscriptions</li>
                            <li>Talent Workshops</li>
                            <li>CPSC Certificates</li>
                            <li>Rating</li>
                            <li>Shop Help</li>
                            <li>Contact Us</li>
                        </ul>
                    </nav>
                    <nav>
                        <h2>Sites</h2>
                        <ul>
                            <li>DC</li>
                            <li>MAD Magazine</li>
                            <li>DC Kids</li>
                            <li>DC Universe</li>
                            <li>DC Power Visa</li>
                        </ul>
                    </nav>
                </div>
                <div class="logo-footer">
                    <img src="../assets/Images/dc-logo-bg.png" alt="">
                </div>
            </div>
        </div>
        <div class="inf">
            <div class="container">
                <button>sign-up now</button>
                <div class="social-icons">
                    <h2>Follow Us</h2>
                    <a href="#"><img src="../assets/Images/footer-facebook.png" alt=""></a>
                    <a href="#"><img src="../assets/Images/footer-twitter.png" alt=""></a>
                    <a href="#"><img src="../assets/Images/footer-youtube.png" alt=""></a>
                    <a href="#"><img src="../assets/Images/footer-pinterest.png" alt=""></a>
                    <a href="#"><img src="../assets/Images/footer-periscope.png" alt=""></a>
                </div>
            </div>
        </div>
    </footer>
</template>

<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

footer {
    width: 100%;

    .sup {
        width: 100%;
        height: 420px;
        background-image: url(../assets/Images/footer-bg.jpg);
        background-size: cover;
        background-repeat: no-repeat;
        @include flex-center;

        .container {
            width: 1200px;
            height: 100%;
            @include flex-between;

            .navigazione {
                display: flex;
                gap: 1rem;
                padding: 3rem 0;
                flex-direction: column;
                flex-wrap: wrap;
                color: #fff;

                nav {
                    h2 {
                        font-family: $text-primary;
                        letter-spacing: 0.1rem;
                        margin-bottom: 1rem;
                    }

                    ul li {
                        margin-bottom: 0.5rem;
                        list-style: none;
                        color: rgb(109, 109, 109);
                        font-size: 0.8rem;
                        cursor: pointer;

                        &:hover {
                            color: #fff;
                        }
                    }
                }
            }

            .logo-footer {
                height: 100%;
                @include flex-center;

                img {
                    width: 550px;
                    object-fit: cover;
                }
            }
        }
    }

    .inf {
        width: 100%;
        height: 100px;
        align-items: center;
        background-color: #303030;
        @include flex-center;

        .container {
            width: 1200px;
            height: 50px;
            @include flex-between;

            button {
                border: 0.3rem solid $primary;
                padding: 0 1rem;
                height: 100%;
                background-color: transparent;
                font-size: 1.1rem;
                text-transform: uppercase;
                color: #fff;
                cursor: pointer;

                &:hover {
                    background-color: $primary;
                }
            }

            .social-icons {
                @include flex-between;
                align-items: center;
                width: 35%;

                h2 {
                    color: $primary;
                    text-transform: uppercase;
                    font-family: $text-primary;
                    letter-spacing: 0.1rem;
                }

                // img{
                //     &:hover{

                //     }
                // }
            }
        }
    }
}
</style>