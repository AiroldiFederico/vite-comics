<script>

export default {
    
name: "NavBar",
  data() {
    return {
        sections: [
        { name: "characters", active: false },
        { name: "comics", active: true },
        { name: "movies", active: false },
        { name: "tv", active: false },
        { name: "games", active: false },
        { name: "collectibles", active: false },
        { name: "video", active: false },
        { name: "fans", active: false },
        { name: "news", active: false },
        { name: "shop", active: false }
      ]
    };
  }
};
    
</script>




<template>
    <div class="main col-10 m-auto">
        <div><img src="\img\dc-logo.png" alt=""></div>
        <nav>
            <ul>
                <li v-for="(section, index) in sections" :key="index" :class="{ 'active': section.active }">
                    <a href="#">{{ section.name }}</a>
                </li>
            </ul>
        </nav>
    </div>
</template>





<style lang="scss" scoped>

.main {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 0.7rem 0rem;
    border-bottom: solid black 1px;

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
        &.active a {
             border-bottom: #0282f9 solid 4px !important;
             color: #0282f9 !important;
         }
            
        }

    }






</style>