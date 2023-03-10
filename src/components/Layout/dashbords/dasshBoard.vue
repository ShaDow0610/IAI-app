<template>
        <headerB :ShowSideBar="ShowSideBar" :Toggeler="ToggleSideBar"/>
        
        <main id="main" class="text-center"  data-aos="fade-in" :class="[!this.ShowSideBar ? this.ShowSideBar:'responsive','responsive2']">
            <pageTitle ShowSideBar />
                    
            <comment/>
          <section class="section">
            
              <div class="row align-items-top">
                  <div class="col-lg-10 offset-lg-1 ">

                  <!-- Default Card -->
                  <dashboardCards v-for="i in 3"/>

                  </div>
                  
                  </div>
            
              <Tools/>
             
          </section>

</main><!-- End #main -->
</template>
<script>
import Card from '@/components/home/Card.vue';
import pageTitle from '@/components/Layout/header/pageTitle.vue';
import headerB from '@/components/Layout/header/headerB.vue';
import dashboardCards from '@/components/Layout/dashboardTools/dashboardCards.vue';
import Tools from '@/components/Layout/dashboardTools/Tools.vue';
import comment from '@/components/Layout/dashboardTools/comment.vue'

export default {
  components:{Card,headerB,dashboardCards,pageTitle,Tools,comment} ,
data(){
return{
    ShowSideBar:false,
    search:true
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
margin-top: 150px ;
}
@media (width>=1099px) {
.shoc{
    flex: 0 0 auto !important;
    width: 33.33333% !important;
}
}
@media (width<=1098px){
.sho{
    flex: 0 0 auto !important;
    width: 50% !important;
    padding-top:0px ;
    padding-bottom:0px ;
}

}



.slide-fade-enter-active {
transition: all 0.5s ease-out;

}
.slide-fade-leave-active {
transition: all 0.5s cubic-bezier(1, 0.5, 0.8, 1);

}
.slide-fade-enter-from,
.slide-fade-leave-to {
transform: translateX(-80px);
opacity: 0;
}

/* .slide-bounce-enter-active{
animation: bounce-in 0.5s ;
}
.slide-bounce-leave-active{
animation: bounce-in 0.5s reverse;
}
@keyframes bounce-in {
0%{
    transform: scale(0);
}
50%{
    transform: scale(1.25);
}
100%{
    transform: scale(1);
}
} */




/* Accordion */
/* .accordion-item {
border: 1px solid #ebeef4;
}

.accordion-button:focus {
outline: 0;
box-shadow: none;
}

.accordion-button:not(.collapsed) {
color: #012970;
background-color: #f6f9ff;
}

.accordion-flush .accordion-button {
padding: 15px 0;
background: none;
border: 0;
}

.accordion-flush .accordion-button:not(.collapsed) {
box-shadow: none;
color: #4154f1;
}

.accordion-flush .accordion-body {
padding: 0 0 15px 0;
color: #3e4f6f;
font-size: 15px;
}
 */

/* #main{
} */
</style>