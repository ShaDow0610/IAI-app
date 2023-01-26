<template>
    <headerB :ShowSideBar="ShowSideBar" :Toggeler="ToggleSideBar"/>
    <main id="main" class="text-center"  data-aos="fade-in" :class="[!this.ShowSideBar ? this.ShowSideBar:'responsive','responsive2']">
        <pageTitle/> 
        <div class="card">
                <div class="card-body">
                <h5 class="card-title">Emplois de temps de la semaine</h5>
                <p>Les <code>Ecris en rouge </code> represente les evaluation controlle continues et de Session Normale</p>
                <!-- Bordered Table -->
                <table class="table">
                    <thead>
                        <tr>
                        <th scope="col">horaire</th>
                        <th scope="col">Lundi</th>
                        <th scope="col">Mardi</th>
                        <th scope="col">Mrecredi</th>
                        <th scope="col">Jeudi</th>
                        <th scope="col">Vendredi</th>
                        <th scope="col">Samedi</th>
                        </tr>
                    </thead>
                    <tbody class="table-group-divider">
                        <tr>
                        <th scope="row">1</th>
                        <td>Mark</td>
                        <td>Otto</td>
                        <td>@mdo</td>
                        </tr>
                        <tr>
                        <th scope="row">2</th>
                        <td>Jacob</td>
                        <td>Thornton</td>
                        <td>@fat</td>
                        </tr>
                        <tr>
                        <th scope="row">3</th>
                        <td colspan="2">Larry the Bird</td>
                        <td>@twitter</td>
                        </tr>
                    </tbody>
                    </table>
                <!-- End Bordered Table -->
            </div>
        </div>
    </main>
</template>
<script>
import headerB from '@/components/Layout/header/headerB.vue';
import pageTitle from '@/components/Layout/header/pageTitle.vue';
export default {
    components:{headerB, pageTitle},
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