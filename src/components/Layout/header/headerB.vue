<template>
    <div class="container">
        <Header>
            <div class="col-12">
                <logo/>
            </div>
            <div class=" row col-12">
                <i class=" toggle-sidebar-btn col-lg-4 px-0 sho shoc" @click="this.Toggeler" :class="[!this.ShowSideBar ? this.ShowSideBar:'bi bi-x-lg ','bi bi-list ']"></i>
                <search-bar :search="search"/>
                <Nav :ShowSearcheBar="chercher"/>

            </div>  
        </Header>
        <transition name="slide-fade">
            <Sidebar v-if="this.ShowSideBar"/>
        </transition>
    </div>
  


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
            console .log(this.search)
        },
    }
}
</script>
<style scoped>

</style>