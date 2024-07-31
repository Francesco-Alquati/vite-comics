<script>
import AppCards from './AppCards.vue';
import AppMainBottom from './AppMainBottom.vue';

export default {
  components: {
    AppCards,
    AppMainBottom,
  },
};
</script>
<template>
    <div class="bg-jumbo"></div>
    <main>
        <div class="container-fluid bg-darkgrey position-relative">
            <div class="row">
                <div class="col-12">
                    <div class="content">
                        <button class="button-current text-uppercase p-absolute-button translate-middle">Current series</button>
                    </div>
                </div>
                <AppCards/>
                <div class="text-center mt-5 mb-3">
                    <button class="button-more text-uppercase">Load more</button>
                </div>
            </div>
        </div>
        <AppMainBottom />
    </main>
</template>
<style lang="scss" scoped>
.bg-jumbo{
    background-image: url('./jumbotron.jpg');
    background-size: cover;
    height: 300px;
}
.bg-darkgrey{
    background-color: rgb(37, 37, 37);
}
.button-current{
    padding: 8px;
    width: 200px;
    border: none;
    background-color: #0281F6;
    color: white;
    font-size: 18px;
    font-weight: bold;
}
.button-more{
    padding: 5px;
    width: 200px;
    border: none;
    background-color: #0281F6;
    color: white;
    font-size: 14px;
}
.p-absolute-button{
    position: absolute;
    top: 0px;
    left: 250px;
}
button:hover{
    background-color: blue;
}

    
</style>