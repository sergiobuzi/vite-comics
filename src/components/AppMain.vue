<script>
    export default{
        name:"AppMain",
        data() {
            return {
            
            }
        }
    }
</script>

<template>
   <main>
       <h1>contenuto va qui</h1>
   </main>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables' as *;

main{
    display: flex;
    justify-content: flex-start;
    align-items: center;
    height: 150px;
    width: 100%;
    background-color: #1d1c1d;
}
</style>