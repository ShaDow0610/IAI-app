<template>
    <div class="row">
      <div class="col-12 card px-0 mb-0">
        <div class="card-header pb-0 px-1  ">
          <h5>Messagerie</h5>
          <div class="row px-2 fixed">
            <div class="col-4 d-flex  justify-content-start px-0">
              <button type="button" class="btn btn-outline-secondary ms-0  iradius ">
                <i class="bi bi-star me-1 marg"></i>
                <span class="intitul marg" >Club</span>
                <span class="badge badge-number ms-1 notif-num1 marg" style="background: rgb(199, 171, 100);">3</span>
              </button>
              <button type="button" class="btn btn-outline-secondary  iradius">
                <i class="bi bi-star me-1 marg"></i>
                <span class="intitul  marg" >Administrateur</span>
                <span class="badge badge-number ms-1 notif-num1 marg" style="background: rgb(199, 171, 100);">3</span>
              </button>
              <button type="button" class="btn btn-outline-secondary  iradius">
                <i class="bi bi-person bxl-airbnb marg"></i>
                 <span class="intitul marg">Messagerie</span>
                 <span class="badge badge-number ms-1 notif-num1 marg" style="background: rgb(199, 171, 100);">3</span>
                </button>
            </div>
            <div class="col-8 d-flex  justify-content-end px-0">
              <button type="button" class="btn btn-outline-secondary radius">
                <i class="bi bi-gear me-1 marg"></i>
                <span class="intitul marg">Parametre</span></button>      
            </div>
          </div>
  
        </div>
        <div class="row h-100  d-flex card-body py-0 pad">
              <div class="col-4 px-1 bgcolor">
                <div class="" v-for="i in 100">
                  <div class="contact  my-2 d-flex justify-content-start" >
                    <img src="/img/BreakingBad55.e723d559.png" alt="Profile" class="img1 rounded-circle " style=""/>
                    <span class="mx-3 my-1 name">bonjour</span>
                    
                  </div>
                </div>
              </div>
              <div class="col-8 messages " >
                <div class="d-flex justify-content-start outmessage" v-for="i in 10">
                  <img  class="img rounded-circle m-2 "  src="@/assets/logo.png"/>
                  <span class="message text-wrap p-1 m-1 d-inline-block h-75" style="max-width:50%">bonjourbonjourbonjourbonjourbonjourbonjourbonjourbonjourbonjourbonjourbonjourbonjourb</span>
                </div>
                <div class="d-flex justify-content-end responese">
                  <img  class="img rounded-circle m-2 "  src="@/assets/img/BreakingBad22.png"/>
                  <div class="message text-wrap p-1 m-1 d-inline-block h-75 " style="max-width:50%">bonsoir</div>
                </div>
              </div>    
                      
        </div>
        <div class="card-footer mx-3 p-0 px-1 fixed-bottom" style="background-color:white">
            <div class="row ">
              <div class="col-4 d-flex justify-content-start" >
                <div class="btn btn-danger me-1">
                  <i class="bi bi-eye-slash "></i>
                </div>
                <div class="btn btn-danger me-1">
                  <i class="bi bi-chat"></i>
                </div>
                <div class="btn btn-danger me-1">
                  <i class="bi bi-trash"></i>
                </div>
                <div class="btn btn-danger me-1">
                  <i class="bi bi-mic-mute"></i>
                </div>
              </div>
              <div class="col-8 m-0 pe-2 ps-0" style="border-left:solid 1px #ced4da;">
                <form class="d-flex justify-content-end pe-1"> 
                  <div class="input-group mb-0 ps-0">
                    <input type="text" class="form-control " placeholder="commenter" aria-label="Recipient's username" aria-describedby="basic-addon2" style="border-top-left-radius:0px ;border-bottom-left-radius:0px ;">
                    <span class="btn btn-success input-group-text" id="basic-addon2" style="border-top-right-radius:0px">
                      <i class="bi bi-chat-right-text"></i>
                    </span>
                  </div>
                </form>
              </div>
            </div>
        </div>
      </div>
    </div>
  </template>
  <script>
  export default {
      setup() {
          
      },
  }
  </script>
  <style scoped>
  .outmessage{
    background-color: #fffcf6;
  }
    
  </style>