<template>
    <headerB :ShowSideBar="ShowSideBar" :Toggeler="ToggleSideBar"/>
        
    <main id="main" class="text-center"  data-aos="fade-in" :class="[!this.ShowSideBar ? this.ShowSideBar:'responsive','responsive2']">
        <pageTitle ShowSideBar />
        <!-- ======= Courses Section ======= -->
        <section id="courses" class="courses main-vote">
            <div class="container d-flex justify-content-center">
                <div class="card text-white bg-dark dashboard-vote" >
                  <div class="card-body">
                    <div class="mb-3">
                      <label for="title" class="form-label">Title</label>
                      <div class="input-group">
                        <input type="text" class="form-control bg-dark text-white" placeholder="Saisir du texte ici">
                        <button class="btn btn-outline-secondary bg-dark text-white" data-bs-toggle="modal" data-bs-target="#exampleModal" type="button" style="z-index:3">
                          <i class="bi bi-image"></i>
                        </button>
                      </div>
                    </div>
                    <!-- Bouton pour ajouter une description -->
                   <div  class="d-inline-block">
                    <button v-if="!showDescription" type="button" class="btn folder-button float-start" @click="showDescription = true">
                        <i class="bi bi-plus"></i> Ajouter une description
                    </button>
                   </div>

                    <!-- Champ de saisie de texte -->
                    <div v-if="showDescription" class="d-inline-block w-100" >
                        <textarea class="form-control my-2 bg-dark text-white"></textarea>
                        <button type="button" class="btn folder-button float-end" @click="showDescription = false">Masquer la description</button>
                    </div>
                  
                    <!-- les autre ici/\ -->
                    <div>
                      <label for="votingType" class="form-label text-white">Type de vote</label>
                      <div class="container">
                        <div class="dropdown float-start w-50">
                          <button class="btn btn-secondary dropdown-toggle w-100" type="button" id="dropdownMenuButton" data-bs-toggle="dropdown" aria-expanded="false">
                            Voting Option
                          </button>
                          <ul class="dropdown-menu dropdown-menu-dark w-100" aria-labelledby="dropdownMenuButton">
                            <li><a class="dropdown-item" href="#"><i class="bi bi-check2"></i> Multiple choice</a></li>
                            <li><a class="dropdown-item" href="#"><i class="bi bi-calendar"></i> Meeting poll</a></li>
                            <li><a class="dropdown-item" href="#"><i class="bi bi-image"></i> Image poll</a></li>
                            <li><a class="dropdown-item" href="#"><i class="bi bi-bar-chart"></i> Ranking poll</a></li>
                          </ul>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>           <!-- Modal -->
            <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel" aria-hidden="true">
                <div class="modal-dialog">
                <div class="modal-content bg-dark text-white">
                    <div class="modal-header">
                    <h5 class="modal-title" id="exampleModalLabel">Titre du modal</h5>
                    <button type="button" class="btn-close btn-close-white rounded" data-bs-dismiss="modal" aria-label="Fermer"></button>
                    </div>
                    <div class="modal-body">
                        <div class="rounded border-dashed p-5 m-5 pb-3">
                            <label for="inputFile" class="btn  btn-lg p-3 mb-2 folder-button pb-3">
                                <i class="bi bi-folder "></i>
                            </label>
                            <p>Cliquez pour télécharger ou déposez un fichier ici </p>
                            <p>JPG, PNG ou GIF. Jusqu'à 4 Mo.</p>
                            <input type="file" class="form-control visually-hidden" id="inputFile">
                        </div>

                      
                    </div>
                    <div class="modal-footer">
                        <button type="button" class="btn btn-secondary w-100" data-bs-dismiss="modal">Annuler</button>
                        </div>  
                    </div>

                </div>
            </div>
            <COMELTools/>
        </section><!-- End Courses Section -->

    </main><!-- End #main -->
</template>

<script>

import Card from '@/components/home/Card.vue';
import pageTitle from '@/components/Layout/header/pageTitle.vue';
import headerB from '@/components/Layout/header/headerB.vue';
import COMELTools from '@/components/Layout/dashboardTools/COMELTools.vue';
export default {
   components:{pageTitle,Card,headerB,COMELTools},
   data(){
    return{
        ShowSideBar:false,
        showDescription: false,
        showDropdown: false,
      selectedOption: { label: "Sélectionner une option", icon: "" },
      options: [
        { label: "Option 1", icon: "bi bi-star-fill" },
        { label: "Option 2", icon: "bi bi-heart-fill" },
        { label: "Option 3", icon: "bi bi-moon-fill" }
      ]
    }
   },
  methods:{
    ToggleSideBar(){
            this.ShowSideBar=!this.ShowSideBar   
        },
    toggleDropdown() {
      this.showDropdown = !this.showDropdown;
    },
    selectOption(option) {
      this.selectedOption = option;
      this.showDropdown = false;
    }
  }
}
</script>
<style>
    .border-dashed{
    border-style: dashed;
    border-color: rgb(27, 27, 27);
    border-width: 3px;
    }
    .dashboard-vote{
        width: 75%;
    }
    .folder-button:hover{
        color: rgb(83, 83, 83);
    }
    .select-vote{
        width:30%;
    }
    @media (max-width:768px){
        .dashboard-vote{
            width: 100%;
        }
        .main-vote{
            margin-left: -30px;
            margin-right: -30px;
        }
        .select-vote{
            width:100%;
        }
    }
</style>

