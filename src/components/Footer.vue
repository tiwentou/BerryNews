<template>
    <div class="footer">
        <ContentFooter :title ="f1Title1" :lien1 ="f1Lien1" :lienName1 ="f1LienName1" :lien2="f2Lien1" :lienName2 ="f2LienName1" :lien3="f3Lien1" :lienName3 ="f3LienName1"/>
        <ContentFooter :title ="f1Title2" :lien1 ="f1Lien2" :lienName1 ="f1LienName2" :lien2="f2Lien2" :lienName2 ="f2LienName2" :lien3="f3Lien2" :lienName3 ="f3LienName2"/>
        <ContentFooter :title ="f1Title3" :lien1 ="f1Lien3" :lienName1 ="f1LienName3" :lien2="f2Lien3" :lienName2 ="f2LienName3" :lien3="f3Lien3" :lienName3 ="f3LienName3"/>
    </div>
</template>

<script>
//import Content from "@/components/commons/content/Content.vue";
import ContentFooter from "@/components/commons/content/ContentFooter.vue";

export default {
    name : 'Footer',
    components:{
        ContentFooter
    },
    data(){
        return{
            f1Title1: 'Me connaitre',
            f1Lien1: 'https://fr.linkedin.com/in/ronald-vitaloni-a07966163',
            f1LienName1: 'CV',
            f2Lien1: 'https://twitter.com/Kota_Studio',
            f2LienName1: 'PortFolio',
            f3Lien1: '',
            f3LienName1: '',

            f1Title2: 'Nous Contacter',
            f1Lien2: '#',
            f1LienName2: 'Email',
            f2Lien2: '#',
            f2LienName2: 'Flux RSS',
            f3Lien2: '',
            f3LienName2: 'Newsletter',

            f1Title3: 'Assistance',
            f1Lien3: '#',
            f1LienName3: 'Mention légal',
            f2Lien3: '#',
            f2LienName3: 'Support',
            f3Lien3: '#',
            f3LienName3: 'Charte de confidentialité'
        };
    }
};
</script>

<style scoped>
    .footer {

        display:flex;
        background-color: #2C2C2C;
        justify-content: space-evenly;
        width: 100%;
        height: 20%;
        color: beige;
    }
</style>
