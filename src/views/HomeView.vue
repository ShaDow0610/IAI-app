<template>
        <Header class="row">
            <div class="col-12">
                <logo class="col-12"/>
            </div>
            <div class="col-12 row align-items-center">
                <i class="bi bi-list toggle-sidebar-btn col-lg-4" @click="ToggleSideBar"></i>
                <search-bar class="col-lg-4"/>
                <Nav class="col-lg-4 ">
                    <Message/>
                    <Notification/>
                    <Profile/>
                </Nav>
            </div>
            
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
import Message from '@/components/header/Message.vue';
import Notification from '@/components/header/Notification.vue';
import Profile from '@/components/header/Profile.vue';
import Sidebar from '@/components/sidebar/Sidebar.vue';

export default {
    components:{ Header ,Logo,SearchBar,Nav,Message ,Notification,Profile,Sidebar} ,
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
   /* .Sidebar{
        transition: 6.5s;
        background: rebeccapurple;
    } */
    .slide-fade-enter-active {
    transition: all 0.3s ease-out;
    }

    .slide-fade-leave-active {
    transition: all 0.4s cubic-bezier(1, 0.5, 0.8, 1);
    }

    .slide-fade-enter-from,
    .slide-fade-leave-to {
    transform: translateX(20px);
    opacity: 0;
    }

</style>
