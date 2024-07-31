<script>
export default {
    data(){
        return{
            links:[
                {
                    label: 'digital comics',
                    img: '/buy-comics-digital-comics.png',
                    url: '#',
                },
                {
                    label: 'dc merchandise',
                    img: '/buy-comics-merchandise.png',
                    url: '#',
                },
                {
                    label: 'subscription',
                    img: '/buy-comics-subscriptions.png',
                    url: '#',
                },
                {
                    label: 'comic shop locator',
                    img: '/buy-comics-shop-locator.png',
                    url: '#',
                },
                {
                    label: 'dc power visa',
                    img: '/buy-dc-power-visa.svg',
                    url: '#',
                },
            ]
        }
    }
}
</script>
<template>
    <div>
        <div class="bg-blue h-130 mx-auto z-index-1">
            <ul class="list-unstyled h-100 text-uppercase d-flex justify-content-center align-items-center">
                <li v-for="link,index in links" :key="index">
                    <img :src="link.img" :class="index === 3 ? 'special-icon' : ''">
                    <a href="link.url">{{ link.label }}</a>
                </li>
            </ul>
        </div>
    </div>
</template>
<style lang="scss" scoped>
ul {
    li{
        margin: 0px 40px;
        font-size: 13px;

        a{
            text-decoration: none;
            color: rgb(255, 255, 255);
        }
    }
}
img{
    width: 40px;
    margin-right: 10px;
}
.h-130{
    height: 130px;
}
.bg-blue{
    background-color: #0281F6;
}
.special-icon{
    width: 30px;
}
.z-index-1{
    position: relative;
    z-index: 1;
}
a:hover{
    color: black;
}
    
</style>