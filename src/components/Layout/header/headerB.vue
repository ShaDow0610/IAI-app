<template>
    <Header class="row align-items-end ">
            <div class="col-12">
                <logo class="align-self-center"/>
            </div>
            <div class=" row col-12">
                <i class=" toggle-sidebar-btn col-lg-4 px-0 sho shoc" @click="this.Toggeler" :class="[!this.ShowSideBar ? this.ShowSideBar:'bi bi-x-lg ','bi bi-list ']"></i>
                <search-bar :search="search" class="col-lg-4 px-0 pb-1 shoc"/>
                <Nav :cherche="chercher" class="d-flex col-lg-4 px-0 pt-1 justify-content-end sho shoc"/>

            </div>  
        </Header>
        <transition name="slide-fade">
            <Sidebar v-if="this.ShowSideBar" class="Sidebar fade-right"/>
        </transition>


</template>
<script>
import Header from '@/components/Layout/header/Header.vue';
import Logo from "@/components/Layout/header/Logo.vue"
import SearchBar from "@/components/Layout/header/SearchBar.vue";
import Nav from '@/components/Layout/header/Nav.vue';
import Sidebar from '@/components/Layout/sidebar/Sidebar.vue';


export default {
    components:{ Header ,Logo,SearchBar,Nav,Sidebar,} ,
    props:['Toggeler','ShowSideBar'],
    data(){
        return{
            search:true,
        }
    },
    methods:{
        chercher(){
            this.search=!this.search
        },
    }
}
</script>
<style scoped>

</style>