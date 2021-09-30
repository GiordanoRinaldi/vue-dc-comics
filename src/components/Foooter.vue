<template>
    <footer>
        <div class="bg-footer">
            <img src="../assets/images/dc-logo-bg.png" alt="">
            <div class="container">
                <div class="footer-links">
                    <div class="first-column">
                        <h3>DC COMICS</h3>
                        <ul>
                            <li v-for="(link, index) in dcComics" :key="index"> <a href="#">{{link}}</a> </li>
                        </ul>
                        <h3 class="section-shop">SHOP</h3>
                        <ul>
                            <li v-for="(link, index) in shop" :key="index"><a href="#">{{link}}</a></li>
                        </ul>
                    </div>
                    <div class="second-column">
                        <h3>DC</h3>
                        <ul>
                            <li v-for="(link, index) in dc" :key="index"><a href="#">{{link}}</a></li>
                        </ul>
                    </div>
                    <div class="third-column">
                        <h3>SITES</h3>
                        <ul>
                            <li v-for="(link, index) in sites" :key="index"><a href="#">{{link}}</a></li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: "Footer",
    data(){
        return{
            dcComics: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News",],
            shop: ["Shop DC", "Shop DC Collectibles",],
            dc: ["Therms Of Use", "Privacy policy (New)", "Ad Choices", "Advertising", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificates", "Ratings", "Shop Help", "Contact Us",],
            sites: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa", ],
        }
    }

}
</script>

<style lang="scss" scoped>
    footer {
        height: 380px;
        background-image: url('../assets/images/footer-bg.jpg');
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

    .footer-links{
        display: flex;
        color: white;

        .section-shop{
            margin-top: 25px;
        }

        div {
            margin: 45px 30px 0 0;
            h3 {
                margin-bottom: 10px;
            }
            ul {
                list-style: none;
                
                a {
                    text-decoration: none;
                    color: #959595;
                }
            }
        }
        
    }
</style>