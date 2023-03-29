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

        <!-- ======= Courses Section ======= -->
        <section id="courses" class="courses main">
            <div class="container" data-aos="fade-up">
                <div class="row" data-aos="zoom-in" data-aos-delay="100" >
                    <Card v-for="i in 50"/>
                </div>
            </div>
            <delegueTools/>
        </section><!-- End Courses Section -->

    </main><!-- End #main -->
</template>

<script>

import Card from '@/components/home/Card.vue';
import pageTitle from '@/components/Layout/header/pageTitle.vue';
import headerB from '@/components/Layout/header/headerB.vue';
import delegueTools from '@/components/Layout/dashboardTools/delegueTools.vue';
export default {
   components:{pageTitle,Card,headerB,delegueTools},
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
<style>
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
        transition: all 0.5s ;

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

    


/*--------------------------------------------------------------
# Courses
--------------------------------------------------------------*/

.toggle-sidebar-inactive  {
    margin-left: 0 !important;
}


.toggle-sidebar-active {
    margin-left: 300px;
}
.courses .course-item {
  border-radius: 5px;
  border: 1px solid #eef0ef;
}

.courses .course-content {
  padding: 15px;
}

.courses .course-content h3 {
  font-weight: 700;
  font-size: 20px;
}

.courses .course-content h3 a {
  color: #37423b;
  transition: 0.3s;
}

.courses .course-content h3 a:hover {
  color: green;
}

.courses .course-content p {
  font-size: 14px;
  color: #777777;
}

.courses .course-content h4 {
  font-size: 14px;
  background: rgb(199, 171, 100);
  padding: 7px 14px;
  color: #fff;
  margin: 0;
}

.courses .course-content .time {
  margin: 0;
  font-weight: 500;
  font-size: 12px;
  color: #37423b;
}

.courses .trainer {
  padding-top: 15px;
  border-top: 1px solid #eef0ef;
}

.courses .trainer .trainer-profile img {
  max-width: 50px;
  border-radius: 50px;
}

.courses .trainer .trainer-profile span {
  padding-left: 10px;
  font-weight: 600;
  font-size: 16px;
  color: #5a6c60;
}

.courses .trainer .trainer-rank {
  font-size: 18px;
  color: #657a6d;
}

</style>
