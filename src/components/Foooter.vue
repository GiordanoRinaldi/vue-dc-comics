<template>
    <footer>
        <div class="bg-footer">
            <img src="@/assets/images/dc-logo-bg.png" alt="">
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer"

}
</script>

<style lang="scss" scoped>
    footer {
        height: 380px;
        background-image: url('~@/assets/images/footer-bg.jpg');
        background-repeat: no-repeat;
        background-size: cover;

        .bg-footer {
            height: 100%;
            overflow: hidden;
            position: relative;
            img{
                position: absolute;
                top: -100px              ;
                right: 320px;
                height: 600px;
            }
        } 
    }
</style>