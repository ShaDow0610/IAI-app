<template>
    <headerB :ShowSideBar="ShowSideBar" :Toggeler="ToggleSideBar"/>
    <main id="main" class="text-center"  data-aos="fade-in" :class="[!this.ShowSideBar ? this.ShowSideBar:'responsive','responsive2']">
        <pageTitle/> 
        <div class="card">
                <div class="card-body">
                <h5 class="card-title">Emplois de temps de la semaine</h5>
                <p>Les <code>Ecris en rouge </code> represente les evaluation controlle continues et de Session Normale</p>
                <!-- Bordered Table -->
                <TimeTable/>
            </div>
        </div>
        <section class="section">
            <div class="row ">
                <div class="col-lg-8">
                    
                     <!-- Default Card -->
                    <TimesTableCards v-for="i in 10">
                        <h5 class="card-title">Emplois de temps de la semaine</h5>
                        <TimeTable/>
                    </TimesTableCards>
                   
                    
                </div>
                <div class="col-lg-4"> 
                    <TimesTabbleExamsCard/>
                </div>
            </div>
            <Tools/>
        </section>

    </main>
</template>
<script>
import headerB from '@/components/Layout/header/headerB.vue';
import pageTitle from '@/components/Layout/header/pageTitle.vue';
import TimesTableCards from '@/components/Layout/Timestable/TimestableCards.vue';
import TimesTabbleExamsCard from '@/components/Layout/Timestable/TimesTableExamsCard.vue'
import TimeTable from '@/components/Layout/Timestable/TimeTable.vue'
 
export default {
    components:{headerB, pageTitle,TimesTableCards,TimesTabbleExamsCard,TimeTable},
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
<style scoped>

</style>