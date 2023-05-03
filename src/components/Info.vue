<script>

    export default{
        name: "Info",
        components: {

        },
        data(){
            return{
                items: [
                    { text: 'Digital Comics', image: '/img/buy-comics-digital-comics.png' },
                    { text: 'DC Merchandising', image: '/img/buy-comics-merchandise.png' },
                    { text: 'Subscription', image: '/img/buy-comics-subscriptions.png' },
                    { text: 'Comic Shop Locator', image: '/img/buy-comics-shop-locator.png' },
                ]

            }
        },
        methods: {
            
        },
    }
    
</script>




<template>
    <div class="main">
        <ul>
            <li v-for="(item, index) in items" :key="index">
              <img :src="item.image" alt="">
              <span>{{ item.text }}</span>
            </li>
        </ul>
    </div>
</template>





<style lang="scss" scoped>

.main {

    background-color:#0282f9ff ;
    color: white;
    padding: 3rem 0;
    
}

ul {
    display: flex;
    justify-content: center;
    align-items: center;

    li {
        margin: 0 2rem;
        text-transform: uppercase;
        font-weight: normal;
    }
}

img {
    width: 3rem;
    height: 3rem;
    margin-right: 1rem;
    object-fit: contain ;
}

</style>