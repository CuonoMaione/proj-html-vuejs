<template>
   <div class="tariff-plans">
        <div class="container">
            <div class="row justify-content-between">
                <div class=" tariff yellow d-flex flex-column text-center justify-content-center align-items-center">
                    <h3>Basic</h3>
                    <h4>99<span>$</span></h4> 
                    <p>5 design Concept</p>
                    <p>Full copyright ownership</p>
                    <p>Art direction</p>
                    <p>Top level creatives</p>
                    <p>No money back</p>
                    <div><button>Learn more <span>&#9656</span></button></div>
                </div>
                <div class=" tariff green d-flex flex-column text-center justify-content-center align-items-center">
                    <h3>Standard</h3>
                    <h4>119<span>$</span></h4> 
                    <p>5 design Concept</p>
                    <p>Full copyright ownership</p>
                    <p>Art direction</p>
                    <p>Top level creatives</p>
                    <p>No money back</p>
                    <div><button>Learn more <span>&#9656</span></button></div>
                </div>
                <div class=" tariff orange d-flex flex-column text-center justify-content-center align-items-center">
                    <h3>Basic</h3>
                    <h4>139<span>$</span></h4> 
                    <p>15 design Concept</p>
                    <p>Full copyright ownership</p>
                    <p>Art direction</p>
                    <p>Top level creatives</p>
                    <p>No money back</p>
                    <div><button>Learn more <span>&#9656</span></button></div>
                </div>
                
            </div>
        </div>
        
   </div>
</template>
<script>
export default {
    name : 'TariffPlans'
}
</script>
<style lang="scss" scoped>
    div.tariff-plans{
        margin-top: 5rem;
        background-image: url(../assets/img/h2-background-img-03.png);
        background-size: cover;
        padding: 5rem 0rem;
    }

    div.container{
        width: 90%;
    }
    div.tariff{
        height: 600px;
        width: calc((100%/3) - 3rem);
        border-radius: 50px;
    }

    .green{
        border:2px solid #e6f3f0;
        background-color: #e6f3f0;
    }
    .yellow{
        border: 2px solid #efca9e;
    }
    .orange{
        border: 2px solid #ea9b82;
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

    p{ 
        font-family: 'Karma', serif;
        color: #6d6e71;
        font-size: 1.2rem;
        
        }
    h3{
        font-size: 1.5rem;
        font-weight: 600;
    }
    h4{
        font-size: 3.5rem;
        font-weight: 600;
        span{
            font-size:1.5rem;
            vertical-align: top;
        }
    }
    button:hover{
        background-color: #80abae;
        transition: 0.5s ease-out;
        color: white;
    }

    aside{
        width: 7%;
        height: 90vh;
        right:0;
        padding-top: 6rem;
        background-color: white;
        position: absolute;
        
    } 
</style>