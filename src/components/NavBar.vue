<script>

export default {
    
name: "NavBar",
  data() {
    return {
      sections: [
        "characters",
        "comics",
        "movies",
        "tv",
        "games",
        "collectibles",
        "video",
        "fans",
        "news",
        "shop"
      ]
    };
  }
};
    
</script>




<template>
    <div class="main">
        <div><img src="\img\dc-logo.png" alt=""></div>
        <nav>
            <ul>
                <li v-for="(section, index) in sections" :key="index">
                    <a href="#">{{ section }}</a>
                </li>
            </ul>
        </nav>
    </div>
</template>





<style lang="scss" scoped>

.main {
    display: flex;
    justify-content: space-around;
    align-items: center;
    margin-top: 0.7rem;
    border-bottom: solid black 1px;
    padding-bottom: 0.7rem;
}

img {
    width: 4rem;
    
}

ul {
    display: flex;
    margin: 0;
    padding: 0;
    li {
        list-style-type: none;
        
        a {
            text-decoration: none;
            text-transform: uppercase;
            font-size: 0.8rem;
            color: darkslategrey;
            padding-bottom: 2rem;
            &:hover {
                border-bottom: #0282f9 solid 4px;
                color: #0282f9;
            }
        }
    }
}




</style>