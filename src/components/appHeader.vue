<template>
    <header>
        
        <div class="header-up">
            <img src="../assets/img/dc-logo.png" alt="logo">
            <ul>
                <li v-for="li in footerList">
                    {{li}}
                </li>
            </ul>

        </div>
        
        <div class="header-down">
            <span>
                -- Content goes here --
            </span>

        </div>
        
    </header>
</template>


<script>
export default {
    name:'appHeader',
    data(){
        return{
            footerList : [
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
    methods:{

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
            height: 70px;
            background-color: $blackColor;
            padding-top: 1.35rem;
            padding-left: 14rem;
            span {
                display: inline-block;
                color: $whiteColor;
                font-size: 1.6rem;
            }
        }
}
    
</style>