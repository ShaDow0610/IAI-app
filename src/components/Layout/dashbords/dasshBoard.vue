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
        <dashboardCards/>
        
        </div>
    </div>
    <Tools/>
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
import Tools from '../dashboardTools/Tools.vue';
import dashboardCards from '@/components/Layout/dashboardTools/dashboardCards.vue';

export default {
components:{ Header ,Logo,SearchBar,Nav,Sidebar,Card,Tools,dashboardCards} ,
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