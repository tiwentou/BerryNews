<template>
    <div class="article">
      <ContentTitle :title='titre'/>
      <ContentBanner :img='image'/>
      <ContentArticle :text='articleText'/>
      <ContentComment />
    </div>
    
</template>

<script>
import ContentTitle from "@/components/commons/content/ContentTitle.vue";
import ContentBanner from "@/components/commons/content/ContentBanner.vue";
import ContentArticle from "@/components/commons/content/ContentArticle.vue";
import ContentComment from "@/components/commons/content/ContentComment.vue";

export default {
  name: 'Main',
  components:{
    ContentTitle,
    ContentBanner,
    ContentArticle,
    ContentComment,
  },
  data(){
    return {
      titre: 'TITRE',
      image: '@/assets/news.png',
      articleText: "Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum."
    };
  }
};
</script>

<style scoped>
.article {
  display : flex;

  margin-left: auto;
  margin-right: auto;
  padding-top:60px;
  flex-direction: column;
  flex-wrap: wrap;

  width: 80%;
  min-height: 1000px;

  color: black;
  background-color: #9C9C9C;
}

</style>
