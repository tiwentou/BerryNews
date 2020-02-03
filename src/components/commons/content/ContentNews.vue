<template>
    <div class="content-news">
        <router-link :to="{name: 'article', params: {id: nbArticle}}">
            <div class="content-news-image">
                <a href=""><img src='@/assets/logo.png'></a>
            </div>
            <div class="content-news-title">
                
                <h2>
                    {{ title }}
                </h2>         
                
            </div>
        </router-link>
    </div>
</template>

<script>

export default {
    name: "ContentNews",
    props: {
        title: String,
        srcImage: String,
        nbArticle: Number
    }
}

</script>

<style scoped>
    .content-news {
        width: 25%;
        background-color: #D92121;
        margin : 5px 2px 25px 2px;
    }

    .content-news .content-news-image{
        background-position : center;
        height: 80%;
    }

    .content-news .content-news-image img{
        height: 100%;
    }

    .content-news .content-news-image img {
        width: 80%;
    }
    .content-news .content-news-title{
        display : flex;
        justify-content: center;
        align-items: center;
        background-color: black;
        color:white;
        height:20%;
    }

    @media only screen and (max-width: 1280px) {
    .content-news {
         width: 80%;
    }
    }

    
</style>