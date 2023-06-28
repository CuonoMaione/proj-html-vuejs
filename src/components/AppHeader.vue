<template>
   <header>
        <nav class="d-flex justify-content-between">
            <img src="../assets/img/logo-img-01.png" alt="" >

            <ul class="d-flex list-group-numbered">
                <li><a href="#">Home</a><div class="dark-pink"></div></li>
                <li><a href="#">Pages</a><div class="light-green"></div></li>
                <li><a href="#">Portfolio</a><div class="brown"></div></li>
                <li><a href="#">Blog</a><div class="gold"></div></li>
                <li><a href="#">Shop</a><div class="light-green"></div></li>
                <li><a href="#">Elements</a><div class="pink"></div></li>
                <li><a href="#"><svg xmlns="http://www.w3.org/2000/svg" width="27" height="27"><circle fill="#C2BF7D" cx="3.5" cy="3.5" r="3.5"/><circle fill="#69A9AA" cx="23.5" cy="3.5" r="3.5"/><circle fill="#E8B068" cx="3.5" cy="23.5" r="3.5"/><circle fill="#EAC78B" cx="13.5" cy="13.5" r="3.5"/><circle fill="#D38366" cx="23.5" cy="23.5" r="3.5"/></svg></a></li>
            </ul>
        </nav>
   </header>
</template>
<script>
export default {
    name: 'AppHeader',

    data() {
        return {
            listLink:[]
        }
    },
}
</script>
<style lang="scss" scoped>

    header{
        
        position: relative;
        width: 100%;
        background-color: white;
        height: 100px;
        
    }

    nav{
        position:fixed;
        width: 100%;
        background-color: white;
        top: 0;
        padding: 2rem 2rem 1rem 2rem;
        border-bottom: 1px solid #e5e5e5;
    }

    li{
        font-weight: 600;
        margin-left: 4rem;
        border-bottom: 2px solid transparent;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
            div{
                width:0%;
                height: 3px;
                
            }
            
    }
    li:first-child{
        div{
        width: 120%;
        height: 3px;
        background-color: #E19074;
        }
    }
    li:hover div{
        width: 120%;
        transition: 0.3s ease;
    }
    img{
        width: 100px;
        object-fit: contain;
    }
    a{
        font-size: 1.1rem;
        font-weight: 500;
        text-decoration: none;
        color: black;
    }

    
</style>