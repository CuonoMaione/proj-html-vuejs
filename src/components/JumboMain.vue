<template>
    <div class="jumbotron">
            <section class="jumbo-text d-flex justify-content-between gap-3">
                <h1>We are Bryson, New York-based art & design studio</h1>
                <p>Here at Bryson it only takes a smidgen of imagination and we’ve already prepared ourselves for future challenges. Take a peek and see if you recognize the trademark ingredients of our work.</p>
            </section>
          </div>
</template>
<script>
export default {
    name : 'JumboMain',
}
</script>
<style lang="scss">
        .jumbotron{
        width: 100%;
        padding: 9rem;
        background-image: url(../assets/img/h2-background-img-02.png);
        background-size: cover;
        
    }
    section.jumbo-text{
        width: 90%;
        margin: 0 auto;
        h1{
            font-size: 3.3rem;
            font-weight: 600;
            width: 100%
            
        }
        p{
            
            font-family: 'Karma', serif;
            color: grey;
            padding-top: 4.5rem;
            width: 100%;
            margin-left: 2rem;
            font-size: 1.1rem;
        }
    }
</style>