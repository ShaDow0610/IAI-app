<template>
    <div>
        <div class="pagepath">
            <nav>
                <ol class="breadcrumb">
                <li class="breadcrumb-item "><a href="index.html"><i class="bi bi-house fs-4"></i></a></li>
                <li class="breadcrumb-item fs-4"> 
                    <router-link :to="'/'+path">
                        / {{this.title}}
                    </router-link> 
                </li>
                </ol>
            </nav>
        </div>
    </div><!-- End Page path -->
    <headerFilter   />


</template>
<script>
import headerFilter from '@/components/Layout/header/headerFilter.vue'
export default {
    components:{headerFilter},
    data(){
        return{
            currentPath:null,
            characterToFind:'/',
            title:null,
            path:null
        }
    },
    methods:{
        showCharactersAfter() {
      let index = this.currentPath.indexOf(this.characterToFind);
      if (index !== -1 && index < this.currentPath.length -1) {
        console.log(this.currentPath.slice(index + 1));
        this.path=this.currentPath.slice(index + 1)
        this.title=this.$route.name
        console.log(this.$route)

      }else {
        console.log('void');
      }
    }
    },
    mounted(){
    console.log(this.$router.currentRoute.value.fullPath) 
    this.currentPath=this.$router.currentRoute.value.fullPath
    console.log(this.currentPath);
    this.showCharactersAfter()
  },
  
}
</script>