<template>
    <main>
        <div class="container-main-up">
            <div class="main-up m-auto align-item-centered">
            <ul>
                <li class="align-item-centered"><img src="../assets/img/buy-comics-digital-comics.png" alt=""> DIGITAL COMICS </li>
                <li class="align-item-centered"><img src="../assets/img/buy-comics-merchandise.png" alt=""> DC MERCHANDISE</li>
                <li class="align-item-centered"><img src="../assets/img/buy-comics-subscriptions.png" alt=""> SUBSCRIPTION</li>
                <li class="align-item-centered"><img src="../assets/img/buy-comics-shop-locator.png" alt=""> COMIC SHOP LOCATOR</li>
                <li class="align-item-centered"><img src="../assets/img/buy-dc-power-visa.svg" alt=""> DC POWER VISA</li>
            </ul>

        </div>
        </div>
        <div class="main-down">
            
            <div class="main-down-left">
                <div class="main-down-left-up">
                    <ul>
                    
                        <li class="title">DC COMICS</li>
                        <li>Characters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>TV</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>

                    </ul>
                </div>
                
                <div class="main-down-left-down">
                    <ul>
                    
                        <li class="title">SHOP</li>
                        <li>Shop DC</li>
                        <li>Shop DC Collectibles</li>

                    </ul>
                </div>

            </div>
    
            <div class="main-down-center">
                <ul>
                    
                    <li class="title">DC</li>
                    <li>Terms Of Use</li>
                    <li>Privacy policy (New)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li> Jobs</li>
                    <li>Subsciptions</li>
                    <li>Talent Workshops</li>
                    <li>CPSC Certicates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                    
                </ul>

            </div>
             
            <div class="main-down-right">
                <ul>
                    <li class="title">SITES</li>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                    
                </ul>

            </div>

            <img src="../assets/img/dc-logo-bg.png" alt="logo-grande">

        </div>
        
    </main>
</template>


<script>
    export default {
        name:'appMain',
        data(){
            return{

            }
        },
        methods:{
    
        }
    
    }
</script>


<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

main{
    
    div.container-main-up{
        background-color: $bluColor;
        div.main-up{
            width: 75%;
            height: 90px;
            ul{
                width:100%;
                @include flexOne();
                li{
                  font-size: 0.7rem;
                  list-style-type: none;
                  color: $whiteColor;
                }
            
                li.title{
                    color: $whiteColor;
                    margin-top: 10px;
                }

                img{
                    width: 1.5rem ;
                    height: 2rem;
                    background-color: $bluColor;
                    margin-right: 5px;
                }
            }
        }

        
    }

    div.main-down{
        background-image: url('../assets/img/footer-bg.jpg');
        height: 285px;
        color: rgb(163, 163, 163);
        display: flex;
        padding-left: 10rem;
        padding-top: 1.1rem;
        font-size: 0.75rem;
        overflow-y: hidden;
        img {
        height: 28rem;
        width: 28rem ;
        margin-left: 20rem;
        margin-top: -5.5rem;
        }
        div.main-down-left{
            margin-right: 1.9rem;
            div.main-down-left-up{
                margin-bottom: 1rem;
                li.title{
                    font-size: 0.8rem;
                    font-weight: bold;
                    margin-bottom: 0.9rem;
                    color: white;
                }

                li{
                list-style-type: none;
                margin-bottom: 0.35rem;
                }
                
            }

            div.main-down-left-down{
                li.title{
                    font-size: 0.8rem;
                    font-weight: bold;
                    margin-bottom: 0.9rem;
                    color: white;
                }
                
                li{
                list-style-type: none;
                margin-bottom: 0.35rem;
                }
                
            }

        }

        div.main-down-center{
            margin-right: 1.9rem;
            li.title{
                font-size: 0.8rem;
                font-weight: bold;
                    margin-bottom: 0.9rem;
            }
            li{
                list-style-type: none;
                margin-bottom: 0.35rem;
            } 
        }

        div.main-down-right{
            margin-right: 1.9rem;
            li.title{
                font-size: 0.8rem;    
                font-weight: bold;
                margin-bottom: 0.9rem;
                color: white;
            }
            li{
                list-style-type: none;
                margin-bottom: 0.35rem;
            }  
        }
    }


}

    
</style>