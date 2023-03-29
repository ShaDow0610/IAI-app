<template>

        
        <main id="main" class="text-center"  data-aos="fade-in" :class="[!this.ShowSideBar ? this.ShowSideBar:'responsive','responsive2']">
            <Messagerie/>

        </main>

</template>
<script>

import Card from '@/components/home/Card.vue';
import pageTitle from '@/components/Layout/header/pageTitle.vue';
import headerB from '@/components/Layout/header/headerB.vue';
import Messagerie from '@/components/Layout/Messageries/Messagerie.vue';

export default {
   components:{pageTitle,Card,headerB,Messagerie},
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
#main {
    margin-top:0px !important;
    padding: 0px;
  }
</style>