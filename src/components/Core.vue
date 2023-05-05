<script>
    import SliderComp from './SliderComp.vue';
    export default{

        name: "Core",
        
        components: {
            SliderComp
        },

        data(){
            return{
               
               Slider: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
              ],

              showPriceAndType: false,

            }
        },
        methods: {
            
        },
    }
    
</script>




<template>
    <div class="main">
        <div id="jumbotron">
            <p>CURRENT SERIES</p>
        </div>
        <div class="col-10 m-auto">
            <div id="slide" >
                <SliderComp  
                v-for="(item, index) in Slider" :key="index"
                :thumb="Slider[index].thumb"
                :series="Slider[index].series"
                :price="Slider[index].price"
                :type="Slider[index].type"
                :show-price-and-type="showPriceAndType"
                />
            </div>
        </div>
        <div id="button">
            <button @click="showPriceAndType = true">LOAD MORE</button>
        </div>
    </div>
</template>





<style lang="scss" scoped>

.main {
    background-color: black;
    padding-bottom: 1rem;

    #jumbotron {
        background-image: url('/img/jumbotron.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        height: 20rem;
        margin-bottom: 2rem;
        position: relative;

        P {
            color: white;
            font-weight: bolder;
            background-color: #0282f9ff;
            display: inline;
            padding: 0.5rem;
            position: absolute;
            bottom: -2.4rem;
            left: 6rem;
        }
    }
    
    #slide {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        color: white;
    }

    #button {

        margin-top: 1rem;
        display: flex;
        justify-content: center;
        button{
            color: white;
            font-weight: bold;
            background-color: #0282f9ff;
            display: inline;
            padding: 0.5rem 2rem;
            border-radius: 4px;
            border: none;
        }
    }
    
}

</style>