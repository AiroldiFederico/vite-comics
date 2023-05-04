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
    <div class="col-10 m-auto">
        <h2> {{ placeholder }} </h2>
    </div>
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