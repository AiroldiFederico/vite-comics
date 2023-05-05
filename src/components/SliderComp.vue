<script>

    export default{
        name: "SliderComp",

        props: {
            thumb: String,
            price: String,
            series: String,
            type: String,
            showPriceAndType: Boolean,
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
        <span>{{series}}</span>
        <span v-if="showPriceAndType">{{type}}</span>
        <span v-if="showPriceAndType">{{price}}</span>
    </div>
</template>





<style lang="scss" scoped>

div {
    width: calc(100% / 6);
    padding: 1.2rem;
    display: flex;
    flex-direction: column;
    img {
        width: 100%;
        aspect-ratio: 1;
        margin-bottom: 1rem;
    }

    span {
        font-weight: normal;
    }
    
}
</style>