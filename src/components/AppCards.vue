<script>
import  comics  from '../components/data/comicsData';
export default {
    data(){
        return{
            comics
        }
    }
}
</script>
<template>
    <div class="card-container">
        <div class="row">
            <div class="col-2 mt-5" v-for="comic in comics" :key="`c-${index}`">
                <div class="comics-card">
                    <img :src="comic.thumb" alt="">
                    <div class="mt-2 text-white fs-13">{{ comic.series }}</div>
                </div>
            </div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
img{
    width: 150px;
    height: 150px;
}
.card-container{
    max-width: 1000px;
    margin: 0 auto;
}
.fs-13{
    font-size: 13px;
}
    
</style>