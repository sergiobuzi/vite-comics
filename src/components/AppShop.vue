<script>
    export default{
        name:"AppShop"
       
    }
</script>

<template>
   <div id="container">
       <ul>
            <li>
                <a href=""><img src="" alt=""></a>
                <div></div>
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
}
</style>