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
                    { text: 'Dc Power Visa', image: '/img/buy-dc-power-visa.svg' },
                ]

            }
        },
        methods: {
            
        },
    }
    
</script>




<template>
    <div class="main">
        <div class="col-10 m-auto">
            <ul>
                <li v-for="(item, index) in items" :key="index">
                  <img :src="item.image" alt="">
                  <span>{{ item.text }}</span>
                </li>
            </ul>
        </div>
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
    justify-content: space-around;
    align-items: center;

    li {
        
        text-transform: uppercase;
        font-weight: normal;
        font-size: small;
    }
}

img {
    width: 3rem;
    height: 3rem;
    margin-right: 0.5rem;
    object-fit: contain ;
}

</style>