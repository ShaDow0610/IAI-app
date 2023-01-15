<template>
        <Header class="">
                <logo class=""/>
                <i class="bi bi-list toggle-sidebar-btn d-flex" @click="ToggleSideBar"></i>
                <search-bar class=" "/>
                <Nav/>
        </Header>
        <transition name="slide-fade">
            <Sidebar v-if="ShowSideBar" class="Sidebar fade-right">

            </Sidebar>
        </transition>
        
</template>

<script>
import Header from '@/components/header/Header';
import Logo from "@/components/header/Logo.vue"
import SearchBar from "@/components/header/SearchBar.vue";
import Nav from '@/components/header/Nav.vue';
import Sidebar from '@/components/sidebar/Sidebar.vue';

export default {
    components:{ Header ,Logo,SearchBar,Nav,Sidebar} ,
    data(){
        return{
            ShowSideBar:false,
        }
    },
    methods:{
        ToggleSideBar(){
            this.ShowSideBar=!this.ShowSideBar
        }
    }
}
</script>
<style>

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
  color: #012970;
}
</style>
