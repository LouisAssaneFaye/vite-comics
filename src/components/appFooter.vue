<template>
    <footer>
        <div class="container-footer m-auto">
            <span>
                SIGN-UP NOW!
            </span>
            <div>
                <ul>
                    <li>FOLLOW US</li>
                    <li v-for="li in footerList">
                        <img src='../assets/img/footer-facebook.png' alt="">
                    </li>
                    
               </ul>
           </div>
        </div>
        
    </footer>
</template>
<script>
export default {
    name:'appFooter',
    data(){
        return{
            footerList: [
                '../assets/img/footer-facebook.png',
                '../assets/img/footer-twitter.png',
                '../assets/img/footer-youtube.png',
                '../assets/img/footer-pinterest.png',
                '../assets/img/footer-periscope.png'
            ]

        }
    },
    methods:{
        
    }
    
}
</script>
<style lang="scss">
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;

footer{
    height: 80px;
    background-color: rgb(53, 53, 53);
    div.container-footer{
        width: 78.5%;
        height: 100%;
        @include flexTwo();
        span{
            border: 2px solid $darkBluColor;
            color: white;
            height: 3rem;
            width: 9rem;
            font-weight: bold;
            line-height: 3rem; 
            text-align: center;
            font-size: 1rem;
        }
        div ul{
            display: flex;
            align-items: center;
            li{
                margin-right: 12px;
                list-style-type: none;
                color: $darkBluColor;
                font-weight: bold;
                font-size: 1rem;
                img{
                    width: 1.5rem;
                    height:1.5rem ;
                }
            }
        }

    }

}

    
</style>