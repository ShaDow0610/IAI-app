<template>
    <p>      
    <button class="btn btn-outline-success  position" type="button" data-bs-toggle="collapse" @click="tools" data-bs-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
        <i class="" :class="[!open ? close:'bi bi-chevron-double-right','bi bi-chevron-double-left']"></i>
    </button>
    </p>
    <div class="collapse" id="collapseExample">
        <Transition name="slide-fade">
            <div class="card card-body position2 p-0 mb-0 bgTools" v-if="show">
                <router-link to="/Chat" class="btn bgBtns fs-3 btn-lg m-2  p-0" data-bs-toggle="tooltip" data-bs-placement="left" title="Tooltip on left">
                    <i class="bi bi-files"></i>
                </router-link>
                <router-link to="stats" class="btn bgBtns fs-4 btn-sm m-2  p-0" data-bs-toggle="tooltip" data-bs-placement="left" title="Tooltip on left">
                    <i class="bi bi-graph-up"></i>
                </router-link>
                <router-link to="/newpost" class="btn bgBtns fs-4 btn-sm m-2  p-0">
                    <i class="bi bi-plus-square"></i>
                </router-link>
                <router-link to="/classroom" class="btn bgBtns fs-4 btn-sm m-2  p-0">
                    <i class="bi bi-person"></i>
                </router-link>
                <button class="btn bgBtns fs-4 btn-sm m-2  p-0" type="button" data-bs-toggle="modal" data-bs-target="#disablebackdrop">
                    <i class="bi bi-list"></i>
                </button>              
                <div class="modal fade modal-marg" id="disablebackdrop" tabindex="-1" data-bs-backdrop="false" style="display: none;" aria-hidden="true">
                    <div class="modal-dialog"> 
                    <div class="modal-content">
                        <div class="modal-header">
                        <h5 class="modal-title">Disabled Backdrop</h5>
                        <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                        </div>
                        <div class="modal-body">
                            Non omnis incidunt qui sed occaecati magni asperiores est mollitia. Soluta at et reprehenderit. Placeat autem numquam et fuga numquam. Tempora in facere consequatur sit dolor ipsum. Consequatur nemo amet incidunt est facilis. Dolorem neque recusandae quo sit molestias sint dignissimos.
                        </div>
                        <div class="modal-footer">
                        <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
                        <button type="button" class="btn btn-primary">Save changes</button>
                        </div>
                    </div>
                    </div>
                </div><!-- End Disabled Backdrop Modal-->
            </div>
        </Transition>  
    </div>
    

</template>
<script>
export default {
    data(){
        return{
            open:false,
            show:false
        }
    },
    methods:{
        tools(){
            this.open=!this.open
            this.show=!this.show
        }
    }
}
</script>
<style scoped>
.modal-marg{
    margin-top: 100px;
    color:black;
}
.bgTools{
  color:rgb(199, 171, 100);
  background: #f6fff6;
  border: solid rgba(199, 171, 100, 0.24);
}
.bgBtns{
    color:rgb(199, 171, 100);
    background-color: rgba(243, 233, 233, 0.411);
    border: solid rgba(0, 0, 0, 0.192) 1px;
}
.bgBtns:hover{
    background: #f6fff6;
    color: green;
    border: solid green 1px;
}
.position{
    position:fixed;
    top:122px;
    right:5px;
    color: black;
   

}
.position2{
    position:fixed;
    top:175px;
    right:5px;
    width: 60px;
}
/*
  Enter and leave animations can use different
  durations and timing functions.
*/
.slide-fade-enter-active {
  transition: all 0.3s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.3s ease-in;
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(20px);
  opacity: 0;
}

</style>