<template>
    <headerB :ShowSideBar="ShowSideBar" :Toggeler="ToggleSideBar"/>
    <main id="main" class="text-center"  data-aos="fade-in" :class="[!this.ShowSideBar ? this.ShowSideBar:'responsive','responsive2']">
      <pageTitle ShowSideBar />
      <!-- ======= Breadcrumbs ======= -->
      <div class="breadcrumbs">
      <div class="container">
          <h2>BIENVENUE</h2>
          <p>ici nous vous presenton les publication les plus recente sur les activiter mener au sein de letblissement</p>
      </div>
      </div><!-- End Breadcrumbs -->
     <section class="section">
          <div class="row">
            <coursCard/>
            <coursCard/>
          </div>
     </section>
    </main>
  
  </template>
  
  <script>
  
  import Card from '@/components/home/Card.vue';
  import pageTitle from '@/components/Layout/header/pageTitle.vue';
  import headerB from '@/components/Layout/header/headerB.vue';
  import coursCard from '@/components/Layout/cours/coursCard.vue'
  
  export default {
     components:{pageTitle,Card,headerB,coursCard},
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