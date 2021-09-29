<template>
    <header>
        <div class="img">
            <img src="@/assets/images/dc-logo.png" alt="logo">
        </div>
        <nav>
            <ul>
                <li v-for="(title, index) in menu" :key="index"><a :href="title.url">{{title.text}}</a></li>
            </ul>
        </nav>
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
header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    .img {
        display: inline-block;
    }
    nav {
        ul {
            display: flex;
            list-style: none;

            a {
                text-decoration: none;
                color: #464646;
                font-weight: 700;
                padding: 0 17px;
            }
        }
    }
}
</style>