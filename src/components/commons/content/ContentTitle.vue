<template>
    <div class="content-title">
        <H1>{{title}}</H1>
    </div>
</template>

<script>

export default {
    name: "ContentTitle",
    props: {
        title : String
    }


}

</script>

<style scoped>
    .content-title {
         display: flex;
         background-color: beige;
         width: 100%;
         height: 80px;
         justify-content: center;      
    }  
</style>