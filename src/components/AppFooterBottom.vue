<script>
export default {
    data(){
        return{
            imgs:[
                {
                    index:'1',
                    url:'/footer-facebook.png'
                },
                {
                    index:'2',
                    url:'/footer-periscope.png'
                },
                {
                    index:'3',
                    url:'/footer-pinterest.png'
                },
                {
                    index:'4',
                    url:'/footer-twitter.png'
                },
                {
                    index:'5',
                    url:'/footer-youtube.png'
                },
            ]
        }
    }
    
}
</script>
<template>
    <div class="bg-grey h-129 z-index-1">
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <div class="d-flex justify-content-center align-items-center h-129">
                        <button class="text-uppercase">sign-up now!</button>
                    </div>
                </div>
                <div class="col-8">
                    <div class="d-flex justify-content-end align-items-center h-129">
                        <h4 class="text-uppercase fs-5 text-blue me-4 mt-2">follow us</h4>
                        <div v-for="img,index in imgs" :key="index">
                            <img :src="img.url">
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
.bg-grey{
    background-color: rgb(45, 45, 45);
}
.h-129{
    height: 129px;
}
.z-index-1{
    position: relative;
    z-index: 1;
}
.text-blue{
    color: #0281F6;
}
button{
    padding: 10px;
    border: 1px solid #0281F6;
    background-color: rgb(45, 45, 45);
    color: white;
}
img{
    margin: 0px 12px;
}
img:hover{
    border-radius: 50%;
    background-color:  white;
}
h4:hover{
    color: blue;
}
button:hover{
    background-color: #0281F6;
}
</style>