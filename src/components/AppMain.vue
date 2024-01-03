<script>
    export default{
        name:"AppMain",
        props:{
            links: Array,
        },

        data() {
            return {
            
            }
        }
    }
</script>

<template>

    <div id="jumbotron"></div>

   <main>

        <div id="container">

            <div id="current">CURRENT SERIES</div>

            <div class="row">

                <div class="card" v-for="(item, i) in links" :key="i">
                    <img :src="item.thumb" alt="" class="img-thumb">
                    <div class="card-text">{{ item.series }}</div>
                
                </div>
                
            </div>
            
        </div>
        
    </main>
    
</template>

<style lang="scss" scoped>
@use '../styles/general.scss' as *;
@use '../styles/partials/variables' as *;

#jumbotron{
    width: 100%;
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-position: top;
    background-repeat: no-repeat;
    background-size: cover;
}

main{
    display: flex;
    justify-content: flex-start;
    align-items: center;
    min-height: 600px;
    width: 100%;
    background-color: #1d1c1d;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;

    #current{
        background-color: $primary;
        font-weight: 600;
        padding: 10px;
        margin-top: -50px;
        margin-bottom: 50px;
        width: 170px;

        
    }

    #container{
        width: 70%;
        margin: auto;
        min-height: 400px;

        .row{
            width: 100%;
            min-height: 450px;
            display: flex;
            flex-wrap: wrap;
            flex-direction: row;
            
            .card{
                width: calc(100% / 6 - 20px);
                min-height: 180px;
                margin: 10px;

                .img-thumb{
                    width: 100%;
                    height: 180px;
                }

                .card-text{
                    margin: 10px;
                }
                
            }
        }
    }
}

</style>