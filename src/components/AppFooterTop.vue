<script>
export default {
    data(){
        return{
            TabList:[
                {
                    titles: 'Dc comics',
                    links:[
                        {
                            label: 'Characters',
                            url: '#',
                        },
                        {
                            label: 'Comics',
                            url: '#',
                        },
                        {
                            label: 'Movies',
                            url: '#',
                        },
                        {
                            label: 'Tv',
                            url: '#',
                        },
                        {
                            label: 'Games',
                            url: '#',
                        },
                        {
                            label: 'Video',
                            url: '#',
                        },
                        {
                            label: 'News',
                            url: '#',
                        },

                    ]
                },
                {
                    titles: 'Shop',
                    links:[
                        {
                            label: 'Shop DC',
                            url: '#',
                        },
                        {
                            label: 'Shop DC Collectibles',
                            url: '#',
                        },
                    ]
                },
                {
                    titles: 'Dc',
                    links:[
                        {
                            label: 'Terms Of Use',
                            url: '#',
                        },
                        {
                            label: 'Privacy police (New)',
                            url: '#',
                        },
                        {
                            label: 'Ad Choices',
                            url: '#',
                        },
                        {
                            label: 'Advertising',
                            url: '#',
                        },
                        {
                            label: 'Jobs',
                            url: '#',
                        },
                        {
                            label: 'Subscriptions',
                            url: '#',
                        },
                        {
                            label: 'Talent Workshops',
                            url: '#',
                        },
                        {
                            label: 'CPSC Certificates',
                            url: '#',
                        },
                        {
                            label: 'Ratings',
                            url: '#',
                        },
                        {
                            label: 'Shop Help',
                            url: '#',
                        },
                        {
                            label: 'Conctac Us',
                            url: '#',
                        },

                    ]
                },
                {
                    titles: 'Sites',
                    links:[
                        {
                            label: 'DC',
                            url: '#',
                        },
                        {
                            label: 'MAD Magazine',
                            url: '#',
                        },
                        {
                            label: 'DC Kids',
                            url: '#',
                        },
                        {
                            label: 'DC Universe',
                            url: '#',
                        },
                        {
                            label: 'DC Power Visa',
                            url: '#',
                        },
                    ]
                },
            ],
        }
    }
}
</script>
<template>
    <div class='h-300 bg-img'>
        <div class="container">
            <div class="row">
                <div class="col-7 d-flex justify-content-center mt-4 position-relative">
                    <div v-for="(title, index) in TabList" :key="title.titles" class="me-5" :class="{ shop: title.titles === 'Shop' }">
                        <h2 class="text-white fs-6 text-uppercase mb-2">{{ title.titles }}</h2>
                        <ul class="list-unstyled">
                          <li v-for="link in title.links" :key="link.label">
                            <a :href="link.url">{{ link.label }}</a>
                          </li>
                        </ul>
                    </div>
                </div>
                <div class="col-5">
                    <div>
                        <img src="/dc-logo-bg.png">
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.h-300{
    height: 300px;
}
.bg-img{
    background-image: url('./footer-bg.jpg');
    background-size: cover;
}
img{
    width: 430px;
    position: relative;
    bottom: 70px;
}
ul {
    li{
        font-size: 11px;

        a{
            text-decoration: none;
            color: rgb(138, 138, 138);
        }
    }
}
.shop {
    position: absolute;
    left: 175px;
    top: 160px;
}
</style>