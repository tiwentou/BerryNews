<template>
    <div class="content-footer">
        <div class="content-footer-title">
            <h4>
                {{ title }}
            </h4>
            <a class="content-a" :href="lien1">{{lienName1}}</a><br/>
            <a class="content-a" :href="lien2">{{lienName2}}</a><br/>
            <a class="content-a" :href="lien3">{{lienName3}}</a>   
        </div>
    </div>
</template>

<script>

export default {
    name: "ContentFooter",
    props: {
        title: String,
        lien1: String,
        lienName1 : String,
        lien2: String,
        lienName2 : String,
        lien3: String,
        lienName3 : String
    }


}

</script>

<style scoped>
    .content-footer {
        display:flex;
        width: 20%;
        max-width: 250px;
        background-color: gray;
        justify-content : center;
        margin : 10px;
        padding :10px;
    }
    .content-footer .content-footer-title .content-a {
        color :black;
    }

</style>