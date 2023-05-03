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
        <div class="lists">
            <ul>
                <h3>DC COMICS</h3>
              <li v-for="item in list1" :key="item">{{ item }}</li>
            </ul>
            <ul>
                <h3> SHOP</h3>
              <li v-for="item in list2" :key="item">{{ item }}</li>
            </ul>
            <ul>
                <h3>DC</h3>
              <li v-for="item in list3" :key="item">{{ item }}</li>
            </ul>
            <ul>
                <h3>SITES</h3>
              <li v-for="item in list4" :key="item">{{ item }}</li>
            </ul>
        </div>
    </div>
</template>





<style lang="scss" scoped>

main {

}

</style>