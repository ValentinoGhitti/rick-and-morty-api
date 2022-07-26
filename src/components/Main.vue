<template>
    <div class="content">
        <div class="container">
            <div class="col-sm-9 mb-5">
                <h1 class="fs-1">Rick And Morty</h1>
                <span>| Find your favorites rick and morty characters</span>
            </div> 
            <div class="col-sm-3"></div>              
        </div>
    </div>
</template>

<script>
export default {
    name: 'Main',
}
</script>

<style scoped>
@font-face {
    font-family: get_schwifity;
    src: url(../../public/font/get_schwifty.ttf);
}

h1 {
    font-family: get_schwifity;
}

#welcome {
    background-image: url(../../public/img/bg.jpg);
    background-position: center;
    background-size: cover;
    height: 100vh;
}
.content {
    display: flex;
    height: 100vh;
    justify-content:space-evenly;
    align-items:flex-start;
    flex-flow: column;
    color: white;

}

@media screen and (max-width: 374px) {
    .span {
        font-size: 1px;
    }
}
</style>