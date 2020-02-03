<template>
    <div class="main">
        <ContentNews :title="articleTitle1" :nbArticle="nbA1"/> 
        <ContentNews :title="articleTitle2" :nbArticle="nbA2"/>
        <ContentNews :title="articleTitle3" :nbArticle="nbA3"/> 
        <ContentNews :title="articleTitle4" :nbArticle="nbA4"/> 
        <ContentNews :title="articleTitle5" :nbArticle="nbA5"/> 
        <ContentNews :title="articleTitle6" :nbArticle="nbA6"/> 
        <ContentNews :title="articleTitle7" :nbArticle="nbA7"/> 
        <ContentNews :title="articleTitle8" :nbArticle="nbA8"/>  
    </div>
    
</template>

<script>
import ContentNews from "@/components/commons/content/ContentNews.vue";


export default {
  name: 'Main',
  components:{
    ContentNews
  },
  data(){
    return {
      articleTitle1: 'ARTICLE 1', nbA1: 1,
      articleTitle2: 'ARTICLE 2', nbA2: 2,
      articleTitle3: 'ARTICLE 3', nbA3: 3,
      articleTitle4: 'ARTICLE 4', nbA4: 4,
      articleTitle5: 'ARTICLE 5', nbA5: 5,
      articleTitle6: 'ARTICLE 6', nbA6: 6,
      articleTitle7: 'ARTICLE 7', nbA7: 7,
      articleTitle8: 'ARTICLE 8', nbA8: 8,
      img1: '@/assets/logo.png'

    };
  }
};
</script>

<style scoped>
.main {
  display : flex;

  margin-left: auto;
  margin-right: auto;
  padding-top:80px;

  flex-wrap: wrap;
  align-items: stretch;

  justify-content: space-evenly;

  width: 80%;
  min-height: 1000px;

  color: black;
  background-color: #9C9C9C;
}

</style>
