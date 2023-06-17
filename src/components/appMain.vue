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
        width: 80%;
        height: 90px;
        ul{
            width:100%;
            @include flexOne();
            li{
              font-size: 0.7rem;
              list-style-type: none;
              color: $whiteColor;
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


}

    
</style>