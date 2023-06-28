<template >
    <footer>
        
        <div class="upper-section">
            <div class="container">
                <div class="row text-section justify-content-between align-items-center">
                    <div class="col-4">
                        <h2>Get in touch and say hello</h2>
                        <p>Lorem ipsum dolor sit amet, consectetuer sociis quis adipiscing elit. Aenean commodo ligula eget dolor. Aenean massa cum. </p>
                    </div>
                    <div class="col-6 ">
                        <textarea class="col-11" placeholder="Comment" value="Comment" name="" id="" cols="30" rows="3"></textarea>
                        <div class="col-12 d-flex justify-content-between">
                            <input type="text" placeholder="Name" class="col-6">
                            <input type="text" placeholder="Email" class="col-6">
                        </div>
                        <div><button>Submit <span>&#9656</span></button></div>
                    </div>
                </div>
                
            </div>
        <aside></aside>
        </div>
        
        <LowerSection/>
        
    </footer>
    
</template>
<script>
import LowerSection from './LowerSection.vue';
export default {
    name: 'AppFooter',
    components:{
        LowerSection,
    }
}
</script>
<style lang="scss" scoped>

    aside{
        width: 7%;
        height: 800px;
        right:0;
        top:0;
        background-color: white;
        position: absolute;
        
    }    

    footer{
        padding-top: 8rem;
        
    }
    div.container{
        width: 90%;
    }
    h2{
        font-size: 3.4rem;
        font-weight: 600;
    } 

    p{ 
        font-family: 'Karma', serif;
        color: #6d6e71;
        font-size: 1.2rem;
        font-weight: 400;
        
        
        }

        .upper-section{
            position: relative;
            margin-bottom: 10rem;
        }
            
        
    .text-section>div {
        padding : 0;
    }

    textarea,input{
        height: 35px;
        border: 0px solid white;
        border-bottom:2px solid #414042;
        font-size: 1.2rem;
        font-family: serif;
        margin-bottom: 3rem;

    }

    textarea{
        width: 100%;
    }
    input{
        width: calc((100%/2) - 2rem)
    }

    div>button{
        text-align: center;
        height: 50px;
        width: 200px;
        border: 1rem;
        border-radius: 40px;
        background-color: white;
        border: 2px solid #80abae;
        font-weight: 500;
        font-family: 'Poppins';
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

    textarea:focus, input:focus{
    outline: none;
    }

   
    
</style>