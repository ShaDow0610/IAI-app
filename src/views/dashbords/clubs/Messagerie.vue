<template>
    <headerB :ShowSideBar="ShowSideBar" :Toggeler="ToggleSideBar"/>
        
        <main id="main" class="text-center"  data-aos="fade-in" :class="[!this.ShowSideBar ? this.ShowSideBar:'responsive','responsive2']">
            
           
            <Messagerie/>

            <tools/>
        </main>

</template>
<script>

import Card from '@/components/home/Card.vue';
import pageTitle from '@/components/Layout/header/pageTitle.vue';
import headerB from '@/components/Layout/header/headerB.vue';
import Tools from '@/components/Layout/dashboardTools/Tools.vue'
import Messagerie from '@/components/Layout/Messageries/Messagerie.vue';

export default {
   components:{pageTitle,Card,headerB,Tools,Messagerie},
   data(){
    return{
        ShowSideBar:false,
    }
   },
  methods:{
    ToggleSideBar(){
            this.ShowSideBar=!this.ShowSideBar
            
        },

  }
}
</script>
<style scoped>
    #main{
        margin-top:120px !important;
        padding: 0px;
    }
</style>