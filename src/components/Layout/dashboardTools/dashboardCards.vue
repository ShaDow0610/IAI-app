<template>
    <div class="card mb-3">
            <div class="row g-0">
              <div class="col-md-4">
                <img src="@/assets/img/BreakingBad3.png" class="img-fluid rounded-start" alt="...">
                <div class="trainer-rankalign-items-center ">
                  
                </div>
                <div class="card mb-0x" style="">
                    <div class="card-body row">
                      <div class="card-title m-0 p-0 col-6">Commentaire</div>
                        <div class="card-subtitle  d-flex  mb-2 text-muted col-6 justify-content-end ">
                          <i class="bi bi-person text-success m-2" ></i>
                          <i class="like bi-heart text-danger m-2" ></i>
                        </div>
                      </div>
                      <div>
                        <div data-bs-spy="scroll" data-bs-target="#navbar-example2" data-bs-root-margin="0px 0px -40%" data-bs-smooth-scroll="true" class="scrollspy-example bg-body-tertiary p-3 rounded-2" tabindex="0">
                          <h4 id="scrollspyHeading1">First heading</h4>
                          <p class="card-text mt-3  ms-3" v-for="i in 10" >
                            <img  class="img"  src="@/assets/logo.png"/>
                            <span class="message p-1 m-1">message</span>
                          </p>
                        </div>

                     
                      </div>
                      <form class="d-flex justify-content-end mt-3"> 
                        <div class="input-group mb-0">
                          <input type="text" class="form-control" placeholder="commenter" aria-label="Recipient's username" aria-describedby="basic-addon2">
                          <span class="btn btn-success input-group-text" id="basic-addon2">
                            <i class="bi bi-chat-right-text"></i>
                          </span>
                        </div>
                      </form>
                  </div>
              </div>
              <div>              
               
              <div class="col-md-8">
              
            </div>
        </div>
    </div>
    </div>
</template>
<style scoped>
  .message{
     border-radius: 15px 15px 15px 0px;
     background:  rgba(181, 179, 179, 0.322);
     
  }
  .img{
    height:8%; 
    width:8%; 
    border-radius:50PX 50PX 50PX 50PX ; 
  }
</style>
