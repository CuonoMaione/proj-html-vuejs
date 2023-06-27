<template>
    <div class="images">
        <div class="container">
            <div class="row">
                <div class="col-6" v-for="element in imageList">
                <img :src="getImagePath(element.image)" :alt="element.name">
                </div>
            </div>
        </div>
   </div>
</template>
<script>
export default {
    name: 'ImageWrapper',
    data() {
        return {
            imageList:[
               {
                name : 'img01',
                image : '../assets/img/port-img-07.jpg'
               },
               {
                name : 'img02',
                image : '../assets/img/port-img-08.jpg'
               },
               {
                name : 'img03',
                image : '../assets/img/port-img-09.jpg'
               },
               {
                name : 'img04',
                image : '../assets/img/port-img-10.jpg'
               },
               {
                name : 'img05',
                image : '../assets/img/port-img-11.jpg'
               },
               {
                name : 'img06',
                image : '../assets/img/port-img-12.jpg'
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
  div.images{
    background-image: url(../assets/img/h2-background-img-04.png);
    background-size: cover;
    background-position: center;
  }
  img{
    height: 650px;
    width: 100%;
  }
  div.col-6{
    padding: 0;
  }
  div.container{
    width: 90%;
    margin-top: 4rem;
  }
 
</style>