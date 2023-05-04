<script>

    export default{
        name: "SliderComp",

        props: {
            thumb: String,
            price: String,
            series: String,
            type: String,
        },

        components: {

        },
        data(){
            return{
               


            }
        },
        methods: {
            
        },
    }
    
</script>




<template>
    <div>
        <img :src="thumb" alt="">
        <!-- <img :src="item.thumb" alt="" v-for="(item, index) in sliderchild" :key="index"> -->
    </div>
</template>





<style lang="scss" scoped>

div {
    
    img {
        width: 5rem;
    }
}
</style>