<script>
export default {
    
}
</script>
<template>
    <div class="bg-jumbo"></div>
    <main>
        <div class="container position-relative">
            <div class="row">
                <div class="col-12">
                    <div class="content">
                        <button class="btn-primary text-uppercase p-absolute-button translate-middle">Current series</button>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>
<style lang="scss" scoped>
.bg-jumbo{
    background-image: url('./jumbotron.jpg');
    background-size: cover;
    height: 300px;
}
main{
    background-color: rgb(37, 37, 37);
    height: 160px;
}
button{
    padding: 8px;
    border: none;
    background-color: #0281F6;
    color: white;
}
.p-absolute-button{
    position: absolute;
    top: 0px;
    left: 250px;
}

    
</style>