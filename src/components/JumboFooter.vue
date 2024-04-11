<template>
    <section>
        <div class="container">
            <div>
                <div>
                    <h5>dc comics</h5>
                    <ul>
                        <li v-for="item in links.dccomics" :key="item.name">
                            <a :href="item.link">{{ item.name }}</a>
                        </li>
                    </ul>
                </div>
                <div>
                    <h5>shop</h5>
                    <ul>
                        <li v-for="item in links.shop" :key="item.name">
                            <a :href="item.link">{{ item.name }}</a>
                        </li>
                    </ul>
                </div>
            </div>
            <div>
                <h5>dc</h5>
                <ul>
                    <li v-for="item in links.dc" :key="item.name">
                        <a :href="item.link">{{ item.name }}</a>
                    </li>
                </ul>
            </div>
            <div>
                <h5>sites</h5>
                <ul>
                    <li v-for="item in links.sites" :key="item.name">
                        <a :href="item.link">{{ item.name }}</a>
                    </li>
                </ul>
            </div>
        </div>

    </section>
</template>

<script>
    export default {
        name: 'JumboFooter.vue',
        data () {
            return {
                links: {
                    dccomics: [
                        {name: 'Characters', link: '#'},
                        {name: 'Comics', link: '#'},
                        {name: 'Movies', link: '#'},
                        {name: 'TV', link: '#'},
                        {name: 'Games', link: '#'},
                        {name: 'Videos', link: '#'},
                        {name: 'News', link: '#'}
                    ],
                    shop: [
                        {name: 'Shop DC', link: '#'},
                        {name: 'Shop DC Collectibles', link: '#'}
                    ],
                    dc: [
                        {name: 'Terms Of Use', link: '#'},
                        {name: 'Privacy policy (New)', link: '#'},
                        {name: 'Ad Choices', link: '#'},
                        {name: 'Advertising', link: '#'},
                        {name: 'Jobs', link: '#'},
                        {name: 'Subscriptions', link: '#'},
                        {name: 'Talent Workshops', link: '#'},
                        {name: 'CPSC Certificates', link: '#'},
                        {name: 'Ratings', link: '#'},
                        {name: 'Shop Help', link: '#'},
                        {name: 'Contact Us', link: '#'}
                    ],
                    sites: [
                        {name: 'DC', link: '#'},
                        {name: 'MAD Magazine', link: '#'},
                        {name: 'DC Kids', link: '#'},
                        {name: 'DC Universe', link: '#'},
                        {name: 'DC Power Visa', link: '#'}
                    ],
                },
            }
        }
    }
    
</script>

<style lang="scss" scoped>

    section {
        background-image: url('/img/dc-logo-bg.png'), url('/img/footer-bg.jpg');
        background-repeat: no-repeat, no-repeat;
        background-size: 600px, cover;
        background-position: calc(100% - 250px), center;
        padding: 60px 0;
        

        .container {
            display: flex;
            justify-content: start;
            align-items: flex-start;
            gap: 20px;
            h5 {
            text-transform: uppercase;
            color: white;
            padding: 10px 0;
            }
            ul {
                list-style: none;
                padding: 0;
                a{
                    text-decoration: none;
                    color: lightgray;
                    font-size: 0.9rem;
                }
            }
        }
    }

</style>