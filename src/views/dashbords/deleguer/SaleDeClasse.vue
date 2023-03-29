<template>
    <headerB :ShowSideBar="ShowSideBar" :Toggeler="ToggleSideBar"/>
        
    <main id="main" class="text-center"  data-aos="fade-in" :class="[!this.ShowSideBar ? this.ShowSideBar:'responsive','responsive2']">
        <pageTitle ShowSideBar />
        <!-- ======= Breadcrumbs ======= -->
        <div class="breadcrumbs">
        <div class="container">
            <h2>BIENVENUE</h2>
            <p>ici nous vous presenton les publication les plus recente sur les activiter mener au sein de letblissement</p>
        </div>
        </div><!-- End Breadcrumbs -->

        <!-- ======= Courses Section ======= -->
        <section id="courses" class="courses main">
            <div class="row ">
                <div class="col-10 p-0 d-flex justify-content-center">
                    <div class="row w-100">
                       <div class=" col-12"> 
                        <h3>fiche d'appel</h3>
                        </div>
                        <div class="fiche">
                            <table class="table able table-bordered">
                                <thead>
                                  <tr>
                                    <th scope="col">#</th>
                                    <th scope="col" class="phoneView">Nom</th>
                                    <th scope="col" class="phoneView">Prenom</th>
                                    <th scope="col" class="phoneView">Age</th>
                                    <th scope="col" class="phoneView">Sexe</th>
                                    <th scope="col" colspan="8">Heure</th>
                                  </tr>
                                </thead>
                                <tbody>
                                  <tr v-for="number in 50" :key="number">
                                    <th scope="row">{{number}}</th>
                                    <td class="phoneView">Mark</td>
                                    <td class="phoneView">Otto</td>
                                    <td class="phoneView">@mdo</td>
                                    <td class="phoneView">@mdo</td>
                                    <td class=" p-0">
                                        <div class=" float-none form-check">
                                        <input class="form-check-input float-none" type="checkbox" value="" id="flexCheckDefault">
                                      </div>
                                    </td>
                                    <td class=" p-0">
                                        <div class=" float-none form-check">
                                        <input class="form-check-input float-none" type="checkbox" value="" id="flexCheckDefault">
                                      </div>
                                    </td>
                                    <td class=" p-0">
                                        <div class=" float-none form-check">
                                        <input class="form-check-input float-none" type="checkbox" value="" id="flexCheckDefault">
                                      </div>
                                    </td>
                                    <td class=" p-0">
                                        <div class=" float-none form-check">
                                        <input class="form-check-input float-none" type="checkbox" value="" id="flexCheckDefault">
                                      </div>
                                    </td>
                                    <td class=" p-0">
                                        <div class=" float-none form-check">
                                        <input class="form-check-input float-none" type="checkbox" value="" id="flexCheckDefault">
                                      </div>
                                    </td>
                                    <td class=" p-0">
                                        <div class=" float-none form-check">
                                        <input class="form-check-input float-none" type="checkbox" value="" id="flexCheckDefault">
                                      </div>
                                    </td>
                                  </tr>
                                </tbody>
                              </table>
                        </div>
                    </div>
                </div>
                <div class="col-2 p-0">
                    <div class="w-100 extra_tools ">
                      <div class="container ms-4 ">
                        <div class="box ms-3 float-end " :class="{'d-block':toolshow}">
                          <div class="d-block ">
                            <div class="btn btn-secondary m-1 p-3 btn-phone rounded-circle" @click="toolshow=!toolshow" :class="{'d-none':!toolshow}">
                              <div class="bi bi-x-lg"></div>
                            </div>
                          </div>
                          <div class="d-block ">
                            <div class="btn btn-danger m-1 p-3 btn-phone"><div class="bi bi-eraser-fill"></div></div>
                            <div class="btn btn-danger m-1 p-3 btn-phone"><div class="bi bi-view-list"></div></div>
                          </div>
                          <div class="d-block">
                            <div class="btn btn-danger m-1 p-3 btn-phone"><div class="bi bi-pencil"></div></div>
                            <div class="btn btn-danger m-1 p-3 btn-phone"><div class="bi bi-gear"></div></div>
                          </div>
                          <div class="d-block">
                            <div class="btn btn-danger m-1 p-3 btn-phone"><div class="bi bi-c-circle"></div></div>
                            <div class="btn btn-danger m-1 p-3 btn-phone"><div class="bi bi-gear"></div></div>
                          </div>
                        </div>
                        <div class="posi " @click="toolshow=!toolshow" :class="{'d-none':toolshow}">
                            <div class="btn btn-outline-secondary rounded-circle"><div class="bi bi-tools"></div></div>
                        </div> 
                      </div>
                    </div>
                </div>
            </div>
            <delegueTools/>
        </section><!-- End Courses Section -->

    </main>
</template>
<script>

import Card from '@/components/home/Card.vue';
import pageTitle from '@/components/Layout/header/pageTitle.vue';
import headerB from '@/components/Layout/header/headerB.vue';
import delegueTools from '@/components/Layout/dashboardTools/delegueTools.vue';
export default {
   components:{pageTitle,Card,headerB,delegueTools},
   data(){
    return{
        ShowSideBar:false,
        number:1,
        toolshow:false
    }
   },
  methods:{
    ToggleSideBar(){
            this.ShowSideBar=!this.ShowSideBar   
        },
    ToggleTools(){
      
    }
  }
}
</script>
<style scoped>
.form-check-input{
    margin-left: -0.5em;
    font-size: 182%;
}
.form-check-input:checked {
    background-color: green;
    border-color: green;
  }
.form-check{
    padding-left: 15px;
}
.form-check-input[type="checkbox"] {
    border-radius: 0;
  }
  .extra_tools{
    
    height: 40%;
    
    
  }
  .box{
    display: none;
    position:fixed;
    bottom: 1px;
  }
  .posi{
    position: fixed;
    bottom: 1%;
    right: 1%;
    display: block;
  }
  .btn-outline-secondary{
    --bs-btn-font-size: 2rem;
  }
  .btn-secondary{
    --bs-btn-font-size: 50%;
  }
  @media (max-width: 768px){
    .btn-secondary{
    --bs-btn-font-size: 123%;
    margin-left: 1px !important;
    margin-right: 15px !important;
    border: none;
    background: rgba(0, 0, 0, 0);
    border-radius: 10px 10px 10px 10px !important;
    
  }
     .btn-outline-secondary{
    --bs-btn-font-size: 1.5 rem;
  }
     .phoneView{
      display: none;
     }
     .box{
      display: ;
      position: fixed;
      left: -10px;
      right: unset;
      margin: 0 !important;
      width: 100%;
      background: rgba(0, 0, 0, 0.466);
      transition-delay: 0.5s;
     }
     .col-10{
      width:100%
     }
     .col-2{
      position: fixed;
      width: 100%;
      display: flex;
     }
     .d-block{
      display: flex !important;
      margin-left: 10px !important;
      margin-right: 30px !important;
      
     }
     .btn-phone{
      padding:20% !important;
      display: flex !important;
      width: 100%;
     }
  }

</style>