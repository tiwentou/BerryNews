<template>
    <div class="header">
        <div class="logo">
            <router-link :to="{name: 'home'}"><h3>BERRYNEWS</h3></router-link>
        </div>
    </div>
</template>

<script>
//import Content from "@/components/commons/content/Content.vue";


export default {
  name: 'Header',

}
</script>

<style scoped>
    .header {
        position:fixed;
        background-color: #2C2C2C;
        color: black;

        width: 100%;
        height: 60px;
        text-align: Left;
    }

    .header .logo {
        display : flex;
        width: 200px;
        height: 60px;
        margin-left:10%;

        justify-content: center;
        align-items: center;
        background-color: gray;
    }
</style>
