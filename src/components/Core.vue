<script>

    export default{
        name: "Core",
        components: {

        },
        data(){
            return{
                placeholder: "--> Content goes here <--",

            }
        },
        methods: {
            
        },
    }
    
</script>




<template>
<div class="main">
    <h2> {{ placeholder }} </h2>
</div>
</template>





<style lang="scss" scoped>

.main {
    background-color: black;
    padding: 3rem 0rem;
    h2 {
        color: white;
        font-weight: bold;
    }
}

</style>