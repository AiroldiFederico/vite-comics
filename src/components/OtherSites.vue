<script>

    export default{
        name: "OtherSites",
        components: {

        },
        data(){
            return{
                list1: [
                    'Characters',
                    'Comics',
                    'Movies',
                    'TV',
                    'Games',
                    'Videos',
                    'News'
                ],

                list2: ['Shop DC', 'Shop DC Collectibles'],

                list3: [
                    'Terms of Use',
                    'Privacy Policy (New)',
                    'Ad Choices',
                    'Advertising',
                    'Jobs',
                    'Subscriptions',
                    'Talent Workshops',
                    'CPSC Certificates',
                    'Ratings',
                    'Shop Help',
                    'Contact Us'
                ],

                list4: ['DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa']
            }
        },
        methods: {
            
        },
    }
    
</script>




<template>
    <div class="main">
        <div class="col-10 m-auto">
            <div class="lists">
                <ul>
                    <h4>DC COMICS</h4>
                  <li v-for="item in list1" :key="item">{{ item }}</li>
                </ul>
                <ul>
                    <h4> SHOP</h4>
                  <li v-for="item in list2" :key="item">{{ item }}</li>
                </ul>
                <ul>
                    <h4>DC</h4>
                  <li v-for="item in list3" :key="item">{{ item }}</li>
                </ul>
                <ul>
                    <h4>SITES</h4>
                  <li v-for="item in list4" :key="item">{{ item }}</li>
                </ul>
            </div>
            <img src="\img\dc-logo-bg.png" alt="">
        </div>
    </div>
</template>





<style lang="scss" scoped>

.main {
    padding: 2rem 0rem;
    background-image: url("/img/footer-bg.jpg");
    color: white;
    position: relative;

    .lists {
        display: flex;
        flex-direction: column;
        flex-wrap: wrap;
        max-width: 40%;
        max-height: 25rem;
    }

    img {
        position: absolute;
        right: 6rem;
        top: -4rem;
        z-index: 0;
    }
}

h4 {
    font-weight: bolder;
}

ul {
    margin-bottom: 2rem;
    li {
        font-weight: lighter;
        margin-left: 0;
    }
}

</style>