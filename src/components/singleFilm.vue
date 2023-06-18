<template>
    <div class="product">
                        <div class="img">
                            <img :src="filmElement.thumb" alt="cover">
                            
                        </div>
                        <div class="description">
                            <span>
                                {{filmElement.series}}
                            </span>
                        </div>
    </div>
</template>
<script>
export default {
    name:'singleFilm',
    props:{
        filmElement: Object,
    }
    
}
</script>
<style lang="scss" scoped>
    
</style>