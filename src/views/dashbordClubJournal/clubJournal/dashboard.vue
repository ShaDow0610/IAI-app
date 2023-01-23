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

  <main id="main" class="main" :class="[!ShowSideBar ? ShowSideBar:'responsive','responsive2']">
        <div class="pagetitle">
        <h1>Cards</h1>
        <nav>
            <ol class="breadcrumb">
            <li class="breadcrumb-item"><a href="index.html">Home</a></li>
            <li class="breadcrumb-item">Components</li>
            <li class="breadcrumb-item active">Cards</li>
            </ol>
        </nav>
        </div><!-- End Page Title -->

        <section class="section">
        <div class="row align-items-top">
            <div class="col-lg-8">

            <!-- Default Card -->
            <div class="card">
                <div class="card-body">
                <h5 class="card-title">Default Card</h5>
                Ut in ea error laudantium quas omnis officia. Sit sed praesentium voluptas. Corrupti inventore consequatur nisi necessitatibus modi consequuntur soluta id. Enim autem est esse natus assumenda. Non sunt dignissimos officiis expedita. Consequatur sint repellendus voluptas.
                Quidem sit est nulla ullam. Suscipit debitis ullam iusto dolorem animi dolorem numquam. Enim fuga ipsum dolor nulla quia ut.
                Rerum dolor voluptatem et deleniti libero totam numquam nobis distinctio. Sit sint aut. Consequatur rerum in.
                </div>
            </div><!-- End Default Card -->

            <!-- Card with header and footer -->
            <div class="card">
                <div class="card-header">Header</div>
                <div class="card-body">
                <h5 class="card-title">Card with header and footer</h5>
                Ut in ea error laudantium quas omnis officia. Sit sed praesentium voluptas. Corrupti inventore consequatur nisi necessitatibus modi consequuntur soluta id. Enim autem est esse natus assumenda. Non sunt dignissimos officiis expedita. Consequatur sint repellendus voluptas.
                Quidem sit est nulla ullam. Suscipit debitis ullam iusto dolorem animi dolorem numquam. Enim fuga ipsum dolor nulla quia ut.
                Rerum dolor voluptatem et deleniti libero totam numquam nobis distinctio. Sit sint aut. Consequatur rerum in.
                </div>
                <div class="card-footer">
                Footer
                </div>
            </div><!-- End Card with header and footer -->

            <!-- Card with an image on left -->
            <div class="card mb-3">
                <div class="row g-0">
                <div class="col-md-4">
                    <img src="@/assets/img/2.png" class="img-fluid rounded-start" alt="...">
                </div>
                <div class="col-md-8">
                    <div class="card-body">
                    <h5 class="card-title">Card with an image on left</h5>
                    <p class="card-text">This is a wider card with supporting text below as a natural lead-in to additional content. This content is a little bit longer.</p>
                    </div>
                </div>
                </div>
            </div><!-- End Card with an image on left -->

            </div>

            <div class="col-lg-4">

            <!-- Card with an image on top -->
            <div class="card">
                <div class="card-body">
                    <div class="card-header">
                        <div class="accordion-item">
                            <h2 class="accordion-header" id="headingOne">
                                <button class="accordion-button collapsed" type="button" data-bs-toggle="collapse" data-bs-target="#collapseOne" aria-expanded="false" aria-controls="collapseOne">
                                Accordion Item #1
                                </button>
                            </h2>
                            <div id="collapseOne" class="accordion-collapse collapse" aria-labelledby="headingOne" data-bs-parent="#accordionExample" style="">
                                <div class="accordion-body">
                                <strong>This is the first item's accordion body.</strong> It is hidden by default, until the collapse plugin adds the appropriate classes that we use to style each element. These classes control the overall appearance, as well as the showing and hiding via CSS transitions. You can modify any of this with custom CSS or overriding our default variables. It's also worth noting that just about any HTML can go within the <code>.accordion-body</code>, though the transition does limit overflow.
                                </div>
                            </div>
                        </div>
                    </div>
                    
                </div>
            </div><!-- End Card with an image on top -->

            <!-- Card with an image on bottom -->
            <div class="card">
                <div class="card-body">
                <h5 class="card-title">Card with an image on bottom</h5>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                </div>
                <img src="assets/img/card.jpg" class="card-img-bottom" alt="...">
            </div><!-- End Card with an image on bottom -->

            </div>

            

            <!-- Special title treatmen -->
            <div class="card text-center">
                <div class="card-header">
                <ul class="nav nav-pills card-header-pills">
                    <li class="nav-item">
                    <a class="nav-link active" href="#">Active</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link" href="#">Link</a>
                    </li>
                    <li class="nav-item">
                    <a class="nav-link disabled" href="#" tabindex="-1" aria-disabled="true">Disabled</a>
                    </li>
                </ul>
                </div>
                <div class="card-body">
                <h5 class="card-title">Special title treatment</h5>
                <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>
                <a href="#" class="btn btn-primary">Go somewhere</a>
                </div>
            </div><!-- End Special title treatmen -->

            </div>

        </section>

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

    

    .toggle-sidebar-btn {
  font-size: 32px;
  padding-left: 10px;
  cursor: pointer;
  color: #1e2023;
}
/* Accordion */
.accordion-item {
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


    /* #main{
    } */
</style>