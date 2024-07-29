<script>
export default {
    data(){
        return{
            links:[
                {
                    index: 1,
                    label: 'digital comics',
                    img: '/buy-comics-digital-comics.png',
                    url: '#',
                },
                {
                    index: 2,
                    label: 'dc merchandise',
                    img: '/buy-comics-merchandise.png',
                    url: '#',
                },
                {
                    index: 3,
                    label: 'subscription',
                    img: '/buy-comics-subscriptions.png',
                    url: '#',
                },
                {
                    index: 4,
                    label: 'comic shop locator',
                    img: '/buy-comics-shop-locator.png',
                    url: '#',
                },
                {
                    index: 5,
                    label: 'dc power visa',
                    img: '/buy-dc-power-visa.svg',
                    url: '#',
                },
            ]
        }
    }
}
</script>
<template lang="">
    <footer>
        <div class="bg-blue h-200 mx-auto">
            <ul class="list-unstyled h-100 text-uppercase d-flex justify-content-center align-items-center">
                <li v-for="link,index in links" :key="index">
                    <img :src="link.img" :class="index === 3 ? 'special-icon' : ''">
                    <a href="link.url">{{ link.label }}</a>
                </li>
            </ul>
        </div>
        <div class="bg-img">
      
        </div>
        <div class="bg-success">
          
        </div>
    </footer>
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
.h-200{
    height: 150px;
}
.bg-blue{
    background-color: #097CEB;
}
.special-icon{
    width: 30px;
}
    
</style>