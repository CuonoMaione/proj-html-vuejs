<template >
    <main>
        <div class="d-flex">
            <div class="content">
                <JumboMain/>

                <ImageWrapper/>
                <WeDo/>
                <TariffPlans/>
            </div>
            <aside>
                <nav class="d-flex flex-column align-items-center justify-content-start">
                <ul class="d-flex flex-column align-content-around gap-3">
                    <li><a href="#"><i class="fa-brands fa-instagram"></i></a></li>
                    <li><a href="#"><i class="fa-brands fa-facebook-f"></i></a></li>
                    <li><a href="#"><i class="fa-brands fa-twitter"></i></a></li>
                    <li><a href="#"><i class="fa-brands fa-pinterest-p"></i></a></li>
                </ul>
                </nav>
            </aside>
        </div>
    </main>
</template>
<script>
import JumboMain from './JumboMain.vue'
import ImageWrapper from './ImageWrapper.vue'
import WeDo from './WeDo.vue';
import TariffPlans from './TariffPlans.vue';
export default {
    name: 'AppMain',
    components:{
    JumboMain,
    ImageWrapper,
    WeDo,
    TariffPlans,
},
}
</script>
<style lang="scss" scoped>

    main{
        overflow: hidden;
        margin-top: 3rem;
        
    }
    div.content{
        width: 100%;
        height: 90hv;
        overflow-y: auto;
        overflow-x: hidden;
        
    }
    
    nav{
        width: 7%;
        height: 90vh;
        overflow: hidden;
        position: fixed;
        top: 20%;
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

    a:hover{
        color: gray;
    }
        
</style>