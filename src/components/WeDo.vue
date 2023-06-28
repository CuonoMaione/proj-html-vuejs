<template>
    <div class="we-do">
        <div class="container">
            <div class="row justify-content-between">
                <div class="col-4">
                    <h2 class="mb-3">What we do? </h2>
                    <p class="mb-5">Lorem ipsum dolor sit amet aenean consectetuer sociis adipiscing elit. Aenean commodo ligula eget dolor pretium quis sem. </p>
                    <div><button> Read more <span>&#9656</span> </button></div>
                </div>
                <div class="col-7">
                        <div class="row">
                            <div class="col-5 d-flex justify-content-center align-items-center mycustom mb-4 ms-5 p-5" v-for="element in wedoList">
                            <img :src="getImagePath(element.image)" alt="">
                            <h3>{{ element.text }}</h3>
                            </div>
                        </div>
                </div>
            </div>
        </div>
    </div>
    <div class="big-image d-flex justify-content-center align-items-center">
        <span class="play-button"></span>
    </div>
</template>
<script>
export default {
    name : 'WeDo',

    data() {
        return {
            wedoList : [
                {
                    text: 'Beatifull illustrations',
                    image: '../assets/img/h2-icon-01.png',
                },
                {
                    text : 'Brand stragies',
                    image: '../assets/img/h2-icon-02.png',
                },
                {
                    text : 'Qualified support',
                    image: '../assets/img/h2-icon-03.png',
                },
                {
                    text : 'Books & magazines',
                    image: '../assets/img/h2-icon-04.png',
                },
            ]
        }
    },
    methods:{
       getImagePath : function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
    },
    },
}
</script>
<style lang="scss" scoped>

    div.we-do{
        margin-top: 12rem;
        margin-bottom: 12rem;
    }
    div.container{
        width: 90%;
    }
    .row>div{
        padding : 0;
    }
    h2{
        font-size: 3rem;
    }

    p{ 
        font-family: 'Karma', serif;
        color: #6d6e71;
        font-size: 1.2rem;
        
        }
    h3{
        width: 50%;
        font-size: 1.4rem;
        font-weight: 600;
        padding-left: 2rem;
    }

    button{
        text-align: center;
        height: 50px;
        width: 200px;
        border: 1rem;
        border-radius: 40px;
        background-color: white;
        border: 2px solid #80abae;
        font-weight: 600;
        
        span{
            font-size: 1.2rem;
            vertical-align:top;
        }
    }
    button:hover{
        background-color: #80abae;
        transition: 0.5s ease-out;
        color: white;
    }
    .big-image{
        padding: 170px 0px;
        height: 580px;
        width: 100%;
        background-image: url(https://bryson.qodeinteractive.com/wp-content/uploads/2019/06/h2-img-2.jpg);
        background-position: center 10px;
        background-repeat: no-repeat;
        position: relative;
    }
    .play-button{
        position: absolute;
        z-index: 2;
        width: 100px;
        height: 100px;
        background-image: url(../assets/img/main-home-video-button-img-01.png);
        background-repeat: no-repeat;
        background-position: center;
        
    }
    .play-button:hover{
        background-image: url(../assets/img/main-home-video-button-img-02.png);
        }
    .mycustom:hover{
        border: 2px solid #e5a85a;
        
        transition: 0.3s ease-in;
    }
    .mycustom{
        border: 2px solid transparent;
        border-radius: 30px;
    }
</style>