<script>
export default {
    data() {
        return {
            menu: [
                {
                    lable: 'characters',
                    url: '#',
                    active: false

                },
                {
                    lable: 'comics',
                    url: '#',
                    active: true

                },
                {
                    lable: 'Movies',
                    url: '#',
                    active: false

                },
                {
                    lable: 'Tv',
                    url: '#',
                    active: false

                },
                {
                    lable: 'Games',
                    url: '#',
                    active: false

                },
                {
                    lable: 'Collectibles',
                    url: '#',
                    active: false

                },
                {
                    lable: 'Videos',
                    url: '#',
                    active: false

                },
                {
                    lable: 'Fans',
                    url: '#',
                    active: false

                },
                {
                    lable: 'News',
                    url: '#',
                    active: false

                },
                {
                    lable: 'Shop',
                    url: '#',
                    active: false

                }
            ]
        }
    }
}
</script>

<template lang="">
    <header>
        <div class="container">
            <img class="logo" src="../assets/Images/dc-logo.png" alt="">
            <nav>
                <ul>
                    <li v-for="(item, index) in menu" key="index" :class="item.active == true ? 'active' : ''">
                        <a  :href="item.url">{{ item.lable }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header {
    width: 100%;
    height: 100px;
    @include flex-center;

    .container {
        width: 1200px;
        @include flex-between;

        .logo {
            margin: 1rem 0;
        }

        nav {
            width: 60%;
            height: 100%;

            ul {
                list-style: none;
                height: 100%;
                @include flex-between;
                ;
                text-transform: uppercase;

                li {
                    height: 100%;
                    border-bottom: 0.3rem solid #fff;

                    &.active,
                    &:hover {
                        border-bottom: 0.3rem solid $primary;
                    }

                    a {
                        align-items: center;
                        @include flex-center;
                        height: 100%;
                        font-family: $text-primary;
                        font-size: 1.1rem;
                        text-decoration: none;
                        color: #000;
                    }
                }
            }
        }
    }
}
</style>