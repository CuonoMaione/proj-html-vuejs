<template >
    <main class="d-flex">
        <div class="content">
         <JumboMain/>
        </div>
        <aside>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Alias officia cupiditate nulla odit aut? Rerum praesentium quo, velit officiis maiores maxime. Quam explicabo eos tempore magnam perferendis. Minima, architecto repellendus!</p>
        </aside>
    </main>
</template>
<script>
import JumboMain from './JumboMain.vue'
export default {
    name: 'AppMain',
    components:{
        JumboMain,
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
        width: 10%;
        height: 90vh;
        overflow: hidden;
        position: fixed;
        right:0;
    }

</style>