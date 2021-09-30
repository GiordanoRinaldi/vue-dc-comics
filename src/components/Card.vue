<template>
    <div class="Card">
        <div class="img-card">
            <img :src="prod.thumb" :alt="prod.series">    
        </div>
        
        <div class="title-card">
            {{prod.series}}
        </div>
    </div>
</template>

<script>
export default {
    name: "Card",
    props: ["prod"]
}
</script>

<style lang="scss" scoped>
    .Card{
        margin: auto;
        width: calc(100% / 6);
    }
    .img-card{
        width: 190px;
        height: 190px;
        overflow: hidden;
            img{
                width: 100%;
                
            }
        
        
    }
</style>