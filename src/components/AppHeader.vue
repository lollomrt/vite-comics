<script>
export default {
    data() {
        return {
            menu: [
                {
                    Lable: 'Characters',
                    url: '#',
                    attivo: 'false'

                },
                {
                    lable: 'comics',
                    url: '#',
                    attivo: 'true'

                },
                {
                    Lable: 'Movies',
                    url: '#',
                    attivo: 'false'

                },
                {
                    Lable: 'Tv',
                    url: '#',
                    attivo: 'false'

                },
                {
                    Lable: 'Games',
                    url: '#',
                    attivo: 'false'

                },
                {
                    Lable: 'Collectibles',
                    url: '#',
                    attivo: 'false'

                },
                {
                    Lable: 'Videos',
                    url: '#',
                    attivo: 'false'

                },
                {
                    Lable: 'Fans',
                    url: '#',
                    attivo: 'false'

                },
                {
                    Lable: 'News',
                    url: '#',
                    attivo: 'false'

                },
                {
                    Lable: 'Shop',
                    url: '#',
                    attivo: 'false'

                }
            ]
        }
    }
}
</script>

<template lang="">
    <header>
        <div class="container">
            <img class="logo" src="" alt="">
            <nav>
                <ul>
                    <li v-for="(item, index) in menu" key="index" :class="item.attivo ? 'active' : ''">
                        <a :href="item.url">{{ item.lable }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style lang="scss">
header {
    ul {
        color: #000;

        a {
            color: #000;
        }
    }
}
</style>