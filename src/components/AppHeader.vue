<template>
   <header class="d-flex justify-content-between p-5">
            <img src="../assets/img/logo-img-01.png" alt="" >

            <ul class="d-flex list-group-numbered">
                <li><a href="#">Home</a></li>
                <li><a href="#">Pages</a></li>
                <li><a href="#">Portfolio</a></li>
                <li><a href="#">Blog</a></li>
                <li><a href="#">Shop</a></li>
                <li><a href="#">Elements</a></li>
                <li><a href="#"><i class="fa-solid fa-braille"></i></a></li>
            </ul>
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

    li{
        font-weight: 600;
        margin-left: 3.5rem;
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