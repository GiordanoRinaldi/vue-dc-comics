<template>
    <header>
        <div class="container">
            <div class="img">
                <img src="../assets/images/dc-logo.png" alt="logo">
            </div>
            <nav>
                <ul>
                    <li v-for="(title, index) in menu" :key="index">
                        <a :class="title.current == true ? 'active' : ''" :href="title.url">
                            {{title.text}}
                            <div v-if="title.current == true" class="line"></div>
                        </a>
                        
                    </li>
                </ul>
            </nav>  
        </div>
    </header>
</template>

<script>
export default {
    name: "Header",
    data() {
        return{
            menu: [
                {
                    text: "CHARACTERS",
                    url: "#",
                    current: false,
                },
                {
                    text: "COMICS",
                    url: "#",
                    current: true,
                },
                {
                    text: "MOVIES",
                    url: "#",
                    current: false,
                },
                {
                    text: "TV",
                    url: "#",
                    current: false,
                },
                {
                    text: "GAMES",
                    url: "#",
                    current: false,
                },
                {
                    text: "COLLECTIBLES",
                    url: "#",
                    current: false,
                },
                {
                    text: "VIDEOS",
                    url: "#",
                    current: false,
                },
                {
                    text: "FANS",
                    url: "#",
                    current: false,
                },
                {
                    text: "NEWS",
                    url: "#",
                    current: false,
                },
                {
                    text: "SHOP",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../assets/style/variables";
.container {
    display: flex;
    height: 120px ;
    justify-content: space-between;
    .img {
        display: inline-block;
        align-self: center;
        width: 80px;
        height: 80px;

        img {
            width: 100% ;
        }
    }
    nav {

        align-self: flex-end;

        ul {
            display: flex;
            list-style: none;

            li {

                a {
                    text-decoration: none;
                    text-align: center;
                    color: #464646;
                    font-weight: 700;
                    margin: 0 17px;
                    display: inline-block;
                }

                .active {
                    color: $mainColor;
                }

                .line {
                    height: 5px;
                    margin-top: 47px;
                    background-color: $mainColor;
                }
            }

            
        }
    }
}
</style>