<template>
    <div class="content-article">
        <p>{{text}}</p>
    </div>
</template>

<script>

export default {
    name: "ContentArticle",
    props: {
        text : String
    }


}

</script>

<style scoped>
    .content-article {
        display: flex;
        background-color: beige;
        width: 100%;
        min-height: 100px;
        justify-content: center; 
        text-align: justify;
    } 

    .content-article p{
        margin: 20px 10px 50px 10px;
    }
</style>