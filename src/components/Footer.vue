<script>

    export default{
        name: "Footer",
        components: {

        },
        data(){
            return{
                images: [
                    '/img/footer-facebook.png',
                    '/img/footer-twitter.png',
                    '/img/footer-youtube.png',
                    '/img/footer-pinterest.png',
                    '/img/footer-periscope.png'
                ]

            }
        },
        methods: {
            
        },
    }
    
</script>




<template>
    <div class="main">
        <div><a href="#">sign-up now</a></div>
        <div>
            <ul>
                <p><a href="#">follow us</a></p>
                <li v-for="(image, index) in images" :key="index">
                  <img :src="image">
                </li>
            </ul>
        </div>
    </div>
</template>





<style lang="scss" scoped>

.main {
    background-color: rgb(49, 49, 49);
    padding: 2rem 0rem;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

a {
    text-transform: uppercase;
    text-decoration: none;
    color: white;
    border: solid 4px #0282f9ff;
    padding: 0.4rem;
}

ul {

    display: flex;
    align-items: center;

    p {
        margin: 0;
        a {
            text-transform: uppercase;
            text-decoration: none;
            color: #0282f9ff;
            border: none;
            
        }
    }

}
</style>