<template >
    <main class="d-flex">
        <div class="content">
            <JumboMain/>
            <ImageWrapper/>
        </div>
        <aside class="d-flex flex-column align-items-center justify-content-start">
            <ul class="d-flex flex-column align-content-around gap-3">
                <li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-facebook-f"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
                <li><a href="#"><i class="fa-brands fa-pinterest-p"></i></a></li>
            </ul>
        </aside>
    </main>
</template>
<script>
import JumboMain from './JumboMain.vue'
import ImageWrapper from './ImageWrapper.vue'
export default {
    name: 'AppMain',
    components:{
        JumboMain,
        ImageWrapper,
    }
}
</script>
<style lang="scss" scoped>

    main{
        overflow: hidden;
        
        
    }
    div.content{
        width: 100%;
        height: 90hv;
        overflow-y: auto;
        overflow-x: hidden;
    }
    aside{
        width: 7%;
        height: 90vh;
        overflow: hidden;
        position: fixed;
        right:0;
        padding-top: 6rem;
        li{
            font-size: 1.25rem;
            

            a{
            text-decoration: none;
            color: black;
            }
        }

        } 
        
</style>