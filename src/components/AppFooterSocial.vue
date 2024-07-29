<script>
export default {
    
}
</script>
<template lang="">
    <div class="bg-grey h-129 z-index-1">
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <div class="d-flex justify-content-center align-items-center h-129">
                        <button class="text-uppercase">sign-up now!</button>
                    </div>
                </div>
                <div class="col-8">
                    <div class="d-flex justify-content-center align-items-center h-129">
                        <h4 class="text-uppercase fs-5 text-blue me-4 mt-2">follow us</h4>
                        <img src="/footer-facebook.png">
                        <img src="/footer-periscope.png">
                        <img src="/footer-pinterest.png">
                        <img src="/footer-twitter.png">
                        <img src="/footer-youtube.png">
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
    margin: 0px 10px;
}
</style>