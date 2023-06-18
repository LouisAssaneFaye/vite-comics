<template>
    <header>
        
        <div class="header-up">
            <img src="../assets/img/dc-logo.png" alt="logo">
            <ul>
                <li v-for="li in headerList">
                    {{li}}
                </li>
            </ul>

        </div>
        
        <div class="header-down">
            
            <div class="jumbotron">
                <img src="../assets/img/jumbotron.jpg" alt="jumbo">
            </div>
            
            <div class="container-product">
                
                <div class="products">
                    
                    <films />

                </div>
                
                <span>
                    LOAD MORE
                </span>
            </div>

        </div>
        
    </header>
</template>


<script>
import films from './films.vue';
export default {
    name:'appHeader',
    data(){
        return{
            headerList : [
                'CHARACTERS',
                'COMICS',
                'MOVIES',
                'TV',
                'GAMES',
                'COLLECTIBLES',
                'VIDEOS',
                'FANS',
                'NEWS',
                'SHOP'
            ]

        }
    },
    components: {
        films
    }
}
</script>


<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

header{
    div.header-up{
        height: 70px;
        @include flexOne();
        img{
            height: 50px;
            width: 50px;
        }
        
        ul>li{
            font-size: 0.6rem;
            list-style-type: none;
            margin-left: 15px;
            
        }

        ul{
            display: flex;
        }
    }

    div.header-down{
            width: 100%;
            background-color: $blackColor;
            div.jumbotron{
                overflow:hidden;
                height: 280px;
                img{
                     width: 100%;
                }
            }

            div.container-product{
                height: 400px;
                @include flexThree();
                div.products{
                    display: flex;
                    flex-wrap: wrap;
                    justify-content: space-between;
                    height: 320px;
                    width: 70%;
                    div.product{
                        width: calc( 100% / 7 );
                        margin-right: 10px;
                        height: 47%;
                        overflow: hidden;
                        div.img{
                            height: 85%;
                            img{
                                width: 100%;
                            }
                        }
                        div.description{
                            display: flex;
                            align-items: center;
                            span{
                                color: $whiteColor;
                                font-size: 0.6rem;
                                background-color: black;
                            }
                            
                        }
                        
                        
                        
                        

                    }
                }
                
            }

            span{
                display: inline-block;
                color: $whiteColor;
                font-weight: bold;
                font-size: 0.9rem;
                background-color: $bluColor;
                width: 12rem;
                height: 2rem;
                line-height: 2rem;
                text-align: center;
                
            }
        }
}
    
</style>