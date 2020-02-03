<template>
    <div class="content-banner">
        <img class ="image" :src='img'>
        <div class="content-author">
            <p class="content-data">AUTHOR+DATE</p>
        </div>
    </div>
</template>

<script>

export default {
    name: "ContentBanner",
    props: {
        img : String
    }


}

</script>

<style scoped>
    .content-banner {
         display: flex;
         flex-wrap: wrap;
         background-color: beige;
         width: 100%;
         height: 200px;
         justify-content: center; 
    }  
    .content-banner .image{
        display: flex;
        width: 100%;
        height: 85%;
    }
    .content-banner .content-author{
        display: flex;
        width: 100%;
        height: 15%;
        justify-content: flex-end;
        align-items: center; 
        background-color: beige;
    }
     .content-banner .content-author .content-data{
         display: flex;
         align-items: center;
         justify-content: center;
         background-color: beige;
         height: 100%;
         width: auto;
         min-width: 30%;
         padding: 0px 10px 0px 10px;
     }
</style>