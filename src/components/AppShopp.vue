<script>
    export default{
        name:"AppShopp",
        data() {
            return {
                items: [
                    {
                        text: "DIGITAL COMICS",
                        url: "#",
                        img: '../public/img/buy-comics-digital-comics.png',
                    },
                    {
                        text: "DC MERCHANDISE",
                        url: "#",
                        img: '../public/img/buy-comics-merchandise.png',
                    },
                    {
                        text: "SUBSCRIPTION",
                        url: "#",
                        img: '../public/img/buy-comics-subscriptions.png',
                    },
                    {
                        text: "COMIC SHOP LOCATOR",
                        url: "#",
                        img: '../public/img/buy-comics-shop-locator.png',
                    },
                    {
                        text: "DC POWER VISA",
                        url: "#",
                        img: '../public/img/buy-dc-power-visa.svg',
                    }
                ],
            }
        }
    }
</script>

<template>
   <div id="container">
       <ul>
            <li v-for="(item, i) in items" :key="i">
                <img :src=item.img alt="" class="shop-img">
                <div>{{ item.text }}</div>
            </li>
       </ul>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables' as *;

#container{
    background-color: $primary;
    color: white;
    width: 100%;
    height: 200px;
    display: flex;
    justify-content: center;
    align-items: center;

    ul{
        list-style-type: none;
        display: flex;
        gap: 30px;
    }

    li{
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 10px;
    }
}



.shop-img{
    color: white;
    width: 50px;
    height: 65px;
}
</style>