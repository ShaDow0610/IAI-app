<template>
    <div class=" p-4 rounded shadow mt-3 post_card  text-start post">
        <!-- author -->
        <div class="d-flex justify-content-between">
          <!-- avatar -->
          <div class="d-flex">
            <img src="@/assets/img/BreakingBad22.png" alt="avatar" class="rounded-circle me-2" style="width: 38px; height: 38px; object-fit: cover">
            <div>
              <p class="m-0 fw-bold">John</p>
              <span class="text-muted fs-7">July 17 at 1:23 pm</span>
            </div>
          </div>
          <!-- edit -->
          <i class="fas fa-ellipsis-h" type="button" id="post1Menu" data-bs-toggle="dropdown" aria-expanded="false"></i>
          <!-- edit menu -->
          <ul class="dropdown-menu border-0 shadow" aria-labelledby="post1Menu">
            <li class="d-flex align-items-center">
              <a class="
                  dropdown-item
                  d-flex
                  justify-content-around
                  align-items-center
                  fs-7
                " href="#">
                Edit Post</a>
            </li>
            <li class="d-flex align-items-center">
              <a class="
                  dropdown-item
                  d-flex
                  justify-content-around
                  align-items-center
                  fs-7
                " href="#">
                Delete Post</a>
            </li>
          </ul>
        </div>
        <!-- post content -->
        <div class="mt-3">
          <!-- content -->
          <p class="">
            Lorem ipsum, dolor sit amet consectetur adipisicing elit.
            Quae fuga incidunt consequatur tenetur doloremque officia
            corrupti provident tempore vitae labore?
          </p>
          <div class="d-flex justify-content-center">
            
            <img src="@/assets/img/BreakingBad5.png" alt="post image" class="img-fluid rounded ">
          </div>
          <!-- likes & comments -->
          <div class="post__comment mt-3 position-relative">
            <!-- likes -->
            <div class="
                d-flex
                align-items-center
                top-0
                start-0
                position-absolute
              " style="height: 50px; z-index: 5">
              <div class="me-2">
                <i class="text-primary fas fa-thumbs-up"></i>
                <i class="text-danger fab fa-gratipay"></i>
                <i class="text-warning fas fa-grin-squint"></i>
              </div>
              <p class="m-0 text-muted fs-7">Phu, Tuan, and 3 others</p>
            </div>
            <!-- comments start-->
            <div class="accordion" id="accordionExample">
              <div class="accordion-item border-0">
                <!-- comment collapse -->
                <h2 class="accordion-header" id="headingTwo">
                  <div class="
                      accordion-button
                      collapsed
                      pointer
                      d-flex
                      justify-content-end
                    " data-bs-toggle="collapse" data-bs-target="#collapsePost1" aria-expanded="false" aria-controls="collapsePost1">
                    <p class="m-0">2 Comments</p>
                  </div>
                </h2>
                <hr>
                <!-- comment & like bar -->
                <div class="d-flex justify-content-around">
                  <div class="
                      dropdown-item
                      rounded
                      d-flex
                      justify-content-center
                      align-items-center
                      pointer
                      text-muted
                      p-1
                    ">
                    <i class="fas fa-thumbs-up me-3"></i>
                    <p class="m-0">Like</p>
                  </div>
                  <div class="
                      dropdown-item
                      rounded
                      d-flex
                      justify-content-center
                      align-items-center
                      pointer
                      text-muted
                      p-1
                    " data-bs-toggle="collapse" data-bs-target="#collapsePost1" aria-expanded="false" aria-controls="collapsePost1">
                    <i class="fas fa-comment-alt me-3"></i>
                    <p class="m-0">Comment</p>
                  </div>
                </div>
                <!-- comment expand -->
                <div id="collapsePost1" class="accordion-collapse collapse" aria-labelledby="headingTwo" data-bs-parent="#accordionExample">
                  <hr>
                  <div class="accordion-body">
                    <!-- comment 1 -->
                    <div class="d-flex align-items-center my-1">
                      <!-- avatar -->
                      <img src="@/assets/img/BreakingBad55.png" alt="avatar" class="rounded-circle me-2" style="
                          width: 38px;
                          height: 38px;
                          object-fit: cover;
                        ">
                      <!-- comment text -->
                      <div class="p-3 rounded comment__input w-100">
                        <!-- comment menu of author -->
                        <div class="d-flex justify-content-end">
                          <!-- icon -->
                          <i class="fas fa-ellipsis-h text-blue pointer" id="post1CommentMenuButton" data-bs-toggle="dropdown" aria-expanded="false"></i>
                          <!-- menu -->
                          <ul class="dropdown-menu border-0 shadow" aria-labelledby="post1CommentMenuButton">
                            <li class="d-flex align-items-center">
                              <a class="
                                  dropdown-item
                                  d-flex
                                  justify-content-around
                                  align-items-center
                                  fs-7
                                " href="#">
                                Edit Comment</a>
                            </li>
                            <li class="d-flex align-items-center">
                              <a class="
                                  dropdown-item
                                  d-flex
                                  justify-content-around
                                  align-items-center
                                  fs-7
                                " href="#">
                                Delete Comment</a>
                            </li>
                          </ul>
                        </div>
                        <p class="fw-bold m-0">John</p>
                        <p class="m-0 fs-7 bg-gray p-2 rounded">
                          Lorem ipsum dolor sit amet, consectetur
                          adipiscing elit.
                        </p>
                      </div>
                    </div>
                    <!-- comment 2 -->
                    <div class="d-flex align-items-center my-1">
                      <!-- avatar -->
                      <img src="@/assets/img/BreakingBad1.png" alt="avatar" class="rounded-circle me-2" style="
                          width: 38px;
                          height: 38px;
                          object-fit: cover;
                        ">
                      <!-- comment text -->
                      <div class="p-3 rounded comment__input w-100">
                        <p class="fw-bold m-0">Jerry</p>
                        <p class="m-0 fs-7 bg-gray p-2 rounded">
                          Lorem ipsum dolor sit amet, consectetur
                          adipiscing elit.
                        </p>
                      </div>
                    </div>
                    <!-- create comment -->
                    <form class="d-flex my-1">
                      <!-- avatar -->
                      <div>
                        <img src="@/assets/img/BreakingBad4.png" alt="avatar" class="rounded-circle me-2" style="width: 38px;height: 38px;object-fit: cover;">
                      </div>
                      <!-- input -->
                      <input type="text" class="form-control border-0 rounded-pill bg-gray" placeholder="Write a comment">
                    </form>
                    <!-- end -->
                  </div>
                </div>
              </div>
            </div>
            <!-- end -->
          </div>
        </div>
      </div>
    <!-- <div class="col-lg-4 col-md-6 d-flex align-items-stretch mt-5" >
        <div class="course-item">
            <img src="@/assets/img/BreakingBad1.png" class="img-fluid " alt="..." style="width:400px; height:400px">
            <div class="course-content">
                <div class="d-flex justify-content-between align-items-center mb-3">
                <h4>Classe</h4>
                <p class="time">02/03/2023<br/> 12h30</p>
            </div>
            <h3><router-link to="/postdetails">Sale de Classe</router-link></h3>
                <p>Et architecto provident deleniti facere repellat nobis iste. Id facere quia quae dolores dolorem tempore.</p>
                <div class="trainer d-flex justify-content-between align-items-center">
                    <div class="trainer-profile d-flex align-items-center">
                        <img src="@/assets/img/1.jpg" class="img-fluid" alt="">
                        <span class=" fw-light fst-italic fs-6">Paul Mibatket</span>
                    </div>
                    <div class="trainer-rank d-flex align-items-center">
                        <i class="bi bi-person text-success fw-light fs-6" ></i><span class="mx-1">{{ numffolowers }}</span>
                        <i class="like fw-light fs-6" @click="Likes" :class="[Clicked ? !Clicked:'bi bi-heart text-success','bi bi-heart-fill text-danger' ]"></i> 
                        <span class="mx-1"> {{ numlikes }}</span>
                    </div>
                </div>
            </div>
        </div>
    </div> End Course Item -->
</template>
<script>
export default {
    data(){
        return{
            Clicked:false,
            numlikes:30,
            numffolowers:70,
        }
    },
    methods:{
        Likes(){
            this.Clicked=!this.Clicked;
            this.numlikes=this.numlikes+1;
        }
    }
}
</script>
<style scoped>

.courses .trainer .trainer-rank i:active{
  font-size:17px ;
}
.like:hover{
    cursor: pointer;
}
@import url('@/assets/css/main.css');

.post{
    background: rgba(255, 255, 255, 0.712);
    box-shadow: 0 .5rem 1rem rgba(0,0,0,.45) !important;
}
</style>