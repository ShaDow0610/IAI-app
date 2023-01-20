<template>
        <Header class="row align-items-end">
            <div class="col-12">
                <logo class="align-self-center"/>
            </div>
            <div class=" row col-12">
                <i class=" toggle-sidebar-btn col-lg-4 px-0 sho shoc" @click="ToggleSideBar" :class="[!ShowSideBar ? ShowSideBar:'bi bi-x-lg ','bi bi-list ']"></i>
                <search-bar :search="search" class="col-lg-4 px-0 pb-1 shoc"/>
                <Nav :cherche="chercher" class="d-flex col-lg-4 px-0 pt-1 justify-content-end sho shoc"/>
            </div>  
        </Header>
        <transition name="slide-fade">
            <Sidebar v-if="ShowSideBar" class="Sidebar fade-right"/>
        </transition>
        
        <main id="main" class="text-center"  data-aos="fade-in" :class="[!ShowSideBar ? ShowSideBar:'responsive','responsive2']">

            <!-- ======= Breadcrumbs ======= -->
            <div class="breadcrumbs">
            <div class="container">
                <h2>Courses</h2>
                <p>Est dolorum ut non facere possimus quibusdam eligendi voluptatem. Quia id aut similique quia voluptas sit quaerat debitis. Rerum omnis ipsam aperiam consequatur laboriosam nemo harum praesentium. </p>
            </div>
            </div><!-- End Breadcrumbs -->

            <!-- ======= Courses Section ======= -->
            <section id="courses" class="courses main">
                <div class="container" data-aos="fade-up">
                    <div class="row" data-aos="zoom-in" data-aos-delay="100" >
                        <Card v-for="i in 10"/>
                    </div>
                </div>
            </section><!-- End Courses Section -->

        </main><!-- End #main -->


        
</template>

<script>
import Header from '@/components/Layout/header/Header.vue';
import Logo from "@/components/Layout/header/Logo.vue"
import SearchBar from "@/components/Layout/header/SearchBar.vue";
import Nav from '@/components/Layout/header/Nav.vue';
import Sidebar from '@/components/Layout/sidebar/Sidebar.vue';
import Card from '@/components/home/Card.vue';

export default {
    components:{ Header ,Logo,SearchBar,Nav,Sidebar,Card} ,
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
        chercher(){
            this.search=!this.search
        }
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

    

    .toggle-sidebar-btn {
  font-size: 32px;
  padding-left: 10px;
  cursor: pointer;
  color: #1e2023;
}
/*--------------------------------------------------------------
# Courses
--------------------------------------------------------------*/

.toggle-sidebar-inactive  {
    margin-left: 0 !important;
}
#main{
    margin-top: 150px;
}

.responsive{
    margin-left: 300px;
    transition: 0.7s;
} 
.responsive2{
 
    transition: 0.7s;
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
