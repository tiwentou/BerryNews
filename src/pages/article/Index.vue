<template>
  <div class="ArticleMain">
    <Header />
    <Article />     
    <Footer />
  </div>
</template>

<script>
    import Header from "@/components/Header.vue"
    import Article from "@/components/Article.vue"
    import Footer from "@/components/Footer.vue"
 
//mon article {{$route.params.id}}

export default {
  name: "articleMain",
  components: {
            Header,
            Article,
            Footer
        }
}
</script>

<style>

</style>
