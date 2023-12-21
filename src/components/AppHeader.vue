<script>
    export default{
        name:"AppHeader",
        data() {
            return {
                links: [
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
                ],
            }
        }
    }
</script>

<template>
    <nav>
        <a href="#" class="logo">
            <img src="../assets/img/dc-logo.png" alt="navbar-logo">
        </a>

        <ul id="nav-items">
            <li v-for="(link, i) in links" :key="i">
                <a href="#" :class="link.current ? 'active' : ''">{{ link.text }}</a>
            </li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables' as *;

nav{
    background-color: #fefeff;
    height: 150px;
    width: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
    font-weight: 600;

    ul{
        list-style: none;
        display: flex;
        gap: 25px;
        color: black;
        cursor: pointer;


        a{
        text-decoration: none;
        color: black;
        padding-bottom: 62px;
        }

        a:hover{
        color: $primary;
        border-bottom: 5px solid $primary;
    }

    }


    .active{
        color: $primary;
        border-bottom: 5px solid $primary;
    }
}



</style>
