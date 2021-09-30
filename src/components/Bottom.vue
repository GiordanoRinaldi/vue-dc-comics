<template>
    <section>
        <div class="container">
            <div v-for="(logo, index) in menu" :key="index" class="logoes">
                <a :href="logo.url">
                    <div class="img">
                        <img :src="require('@/assets/images/'+ logo.img)" :alt="logo.text">
                    </div>
                    <div class="text">
                       {{logo.text}} 
                    </div>
                </a>
                
            </div>
        </div>
    </section>
  
</template>

<script>
export default {
    name: "Bottom",
    data() {
        return{
            menu: [
                {
                    text: "DIGITAL COMICS", 
                    url: "#",
                    current: false,
                    img: "buy-comics-digital-comics.png"
                },
                {
                    text: "DC MERCHANDISE", 
                    url: "#",
                    current: false,
                    img: "buy-comics-merchandise.png"
                },
                {
                    text: "SUBSCRIPTION", 
                    url: "#",
                    current: false,
                    img: "buy-comics-subscriptions.png"
                },
                {
                    text: "COMIC SHOP LOCATOR", 
                    url: "#",
                    current: false,
                    img: "buy-comics-shop-locator.png"
                },
                {
                    text: "DC POWER VISA", 
                    url: "#",
                    current: false,
                    img: "buy-dc-power-visa.svg"
                } 
                

            ]
        }
    }


}
</script>

<style lang="scss" scoped>
    section {
         background-color: #0282f9;;


        .container {
                height: 155px;
                display: flex;
                justify-content: space-around;
                align-items: center;

        }

    }

    .logoes {
        height: 60px;
        a {
            display: flex;
            align-items: center;
            text-decoration: none;
            color: white;
            .img {
                height: 60px;
                margin-right: 10px ;
                img {
                    height: 100%;
                }
            }
        } 
    }

    .logoes:last-child{
        a{
            margin-top: 13px;
            .img{
                height: 35px;
            }
        }
    }
    

</style>