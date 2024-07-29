<script>
export default {
    data(){
        return{
            links:[
                {
                    label: 'Characters',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Comics',
                    url: '#',
                    current: true,
                },
                {
                    label: 'Movies',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Tv',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Games',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Collectibles',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Video',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Fans',
                    url: '#',
                    current: false,
                },
                {
                    label: 'News',
                    url: '#',
                    current: false,
                },
                {
                    label: 'Shop',
                    url: '#',
                    current: false,
                },
            ]
        }
    }
}
</script>
<template lang="">
    <header>
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <div class="text-center">
                        <img src="/dc-logo.png" />
                    </div>
                </div>
                <div class="col-8">
                    <ul class="list-unstyled h-100 text-uppercase d-flex justify-content-center align-items-center">
                        <li v-for="link,index in links" :key="index" :class="link.current ? 'active' : ''">
                            <a href="link.url">{{ link.label}}</a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </header>
</template>
<style lang="scss" scoped>
    ul {
        li{
            margin: 0px 10px;
            font-size: 13px;

            a{
                text-decoration: none;
                color: black;
            }
        }
        .active a{
            color: blue;
        }
    }
</style>