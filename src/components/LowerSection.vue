<template>
    <div class="lower-section">
        <div class="container">
            <div class="row">
                <div class="col-12 text-center">
                    <h1>Bryson</h1>
                </div>
                <div class="col-12 text-center">
                    <p class="mt-3">Sometimes doing something seemingly demanding turns out to be fun.
                    Here’s the proof - Bryson, your brand new portfolio.
                    </p>
                </div>
                <div class="col-12">
                    <div class="row justify-content-center brands gap-3 mt-4" >
                        <div class="col-3 ig"><i class="fa-brands fa-instagram"></i></div>
                        <div class="col-3 fb"><i class="fa-brands fa-facebook-f"></i></div>
                        <div class="col-3 tw"><i class="fa-brands fa-twitter"></i></div>
                        <div class="col-3 pt"><i class="fa-brands fa-pinterest-p"></i></div>
                    </div>
                </div>
            </div>
        </div>
    <aside></aside>
    </div>
    
</template>

<script>
export default {
    name: 'LowerSection',
}
</script>

<style lang="scss" scoped>
    .lower-section{
        position: relative;
        height:400px;
        width:100%;
        background-color:#e4eeed;
        background-image: url(../assets/img/h2-footer-img-01.jpg);
        padding-top: 9rem;        

    }
    aside{
        width: 7%;
        height: 350px;
        right:0;
        top:0;
        background-color:#e4eeed;
        
        position: absolute;
        
    }
    div.container{
        width: 40%;
    }
    p{ 
        font-family: 'Karma', serif;
        color: #6d6e71;
        font-size: 1rem;
        
        }

    i.fa-instagram{
        color: white;
        font-size: 1.5rem;
    }    

    .brands>div{
        width: 35px;
        height: 35px;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 50%;
        color: white;
    }
    div.ig{
        background-color: #69a9aa;
    }
    div.fb{
        background-color: #f7d293;
    }
    div.tw{
        background-color: #f7bca8;
    }
    div.pt{
        background-color: #d8d597;
    }

    h1{
        font-weight: 600;
        font-size: 2.3rem;
    }
</style>