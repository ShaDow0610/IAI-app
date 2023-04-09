<template>
   <nav class="header-nav page d-flex px-0 pt-1 justify-content-end sho shoc">
      <ul class="d-flex align-items-center">

        <li class="nav-item showSearchBar" v-if="connected">
          <div class="nav-link nav-icon search-bar-toggle "  @click="this.ShowSearcheBar" href="#">
            <i class="bi bi-search" ></i>
          </div>
        </li><!-- End Search Icon-->

        <li class="nav-item dropdown" v-if="connected">

          <div class="nav-link nav-icon" href="#" data-bs-toggle="dropdown" >
            <i class="bi bi-bell"></i>
            <span class="badge  badge-number" style="background:rgb(199, 171, 100)">4</span>
          </div><!-- End Notification Icon -->

          <ul class="dropdown-menu dropdown-menu-end dropdown-menu-arrow notifications">
            <li class="dropdown-header">
              You have 4 new notifications
              <router-link to="/messagerie"><span class="badge rounded-pill bg-primary p-2 ms-2">View all</span></router-link>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li class="notification-item">
              <i class="bi bi-exclamation-circle text-warning"></i>
              <div>
                <h4>Lorem Ipsum</h4>
                <p>Quae dolorem earum veritatis oditseno</p>
                <p>30 min. ago</p>
              </div>
            </li>

            <li>
              <hr class="dropdown-divider">
            </li>

            <li class="notification-item">
              <i class="bi bi-x-circle text-danger"></i>
              <div>
                <h4>Atque rerum nesciunt</h4>
                <p>Quae dolorem earum veritatis oditseno</p>
                <p>1 hr. ago</p>
              </div>
            </li>

            <li>
              <hr class="dropdown-divider">
            </li>

            <li class="notification-item">
              <i class="bi bi-check-circle text-success"></i>
              <div>
                <h4>Sit rerum fuga</h4>
                <p>Quae dolorem earum veritatis oditseno</p>
                <p>2 hrs. ago</p>
              </div>
            </li>

            <li>
              <hr class="dropdown-divider">
            </li>

            <li class="notification-item">
              <i class="bi bi-info-circle text-primary"></i>
              <div>
                <h4>Dicta reprehenderit</h4>
                <p>Quae dolorem earum veritatis oditseno</p>
                <p>4 hrs. ago</p>
              </div>
            </li>

            <li>
              <hr class="dropdown-divider">
            </li>
            <li class="dropdown-footer">
              <a href="#">Show all notifications</a>
            </li>

          </ul><!-- End Notification Dropdown Items -->

        </li><!-- End Notification Nav -->

        <li class="nav-item dropdown" v-if="connected" >

          <div class="nav-link nav-icon" href="#" data-bs-toggle="dropdown">
            <i class="bi bi-chat-left-text"></i>
            <span class="badge  badge-number" style="background:rgb(199, 171, 100)">3</span>
          </div><!-- End Messages Icon -->

          <ul class="dropdown-menu dropdown-menu-end dropdown-menu-arrow messages">
            <li class="dropdown-header">
              You have 3 new messages
              <router-link to="/messagerie" ><span class="badge rounded-pill bg-primary p-2 ms-2">View all</span></router-link>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li class="message-item">
              <a href="#">
                <img src="@/assets/img/BreakingBad4.png" alt="" class="rounded-circle">
                <div>
                  <h4>Maria Hudson</h4>
                  <p>Velit asperiores et ducimus soluta repudiandae labore officia est ut...</p>
                  <p>4 hrs. ago</p>
                </div>
              </a>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li class="message-item">
              <a href="#">
                <img src="@/assets/img/BreakingBad5.png" alt="" class="rounded-circle">
                <div>
                  <h4>Anna Nelson</h4>
                  <p>Velit asperiores et ducimus soluta repudiandae labore officia est ut...</p>
                  <p>6 hrs. ago</p>
                </div>
              </a>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li class="message-item">
              <a href="#">
                <img src="@/assets/img/BreakingBad33.png" alt="" class="rounded-circle">
                <div>
                  <h4>David Muldon</h4>
                  <p>Velit asperiores et ducimus soluta repudiandae labore officia est ut...</p>
                  <p>8 hrs. ago</p>
                </div>
              </a>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li class="dropdown-footer">
              <a href="#">Show all messages</a>
            </li>

          </ul><!-- End Messages Dropdown Items -->

        </li><!-- End Messages Nav -->

        <li class="nav-item dropdown pe-3" v-if="connected">

          <div class="nav-link nav-profile d-flex align-items-center pe-0"  data-bs-toggle="dropdown">
            <img src="@/assets/img/BreakingBad55.png" alt="Profile" class="rounded-circle">
            <span class="d-none d-md-block dropdown-toggle ps-2">K. Anderson</span>
          </div><!-- End Profile Iamge Icon -->

          <ul class="dropdown-menu dropdown-menu-end dropdown-menu-arrow profile">
            <li class="dropdown-header">
              <h6>Kevin Anderson</h6>
              <span>Web Designer</span>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li>
              <a class="dropdown-item d-flex align-items-center" href="users-profile.html">
                <i class="bi bi-person"></i>
                <span>My Profile</span>
              </a>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li>
              <a class="dropdown-item d-flex align-items-center" href="users-profile.html">
                <i class="bi bi-gear"></i>
                <span>Account Settings</span>
              </a>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li>
              <a class="dropdown-item d-flex align-items-center" href="pages-faq.html">
                <i class="bi bi-question-circle"></i>
                <span>Need Help?</span>
              </a>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li>
              <a class="dropdown-item d-flex align-items-center" href="#">
                <i class="bi bi-box-arrow-right"></i>
                <span>Sign Out</span>
              </a>
            </li>

          </ul><!-- End Profile Dropdown Items -->
        </li><!-- End Profile Nav -->

        <li class="nav-item dropdown pe-3" v-if="!connected">

          <a class="nav-link nav-log-in d-flex align-items-center pe-0" href="" data-bs-toggle="dropdown">
            <i class="bi bi-box-arrow-in-right "></i>
            <span class="d-none d-md-block ps-2">Se Connecter</span>
          </a><!-- End Profile Iamge Icon -->

          <ul class="dropdown-menu dropdown-menu-end dropdown-menu-arrow profile">
            <!-- <li class="dropdown-header">
              <h6>Kevin Anderson</h6>
              <span>Web Designer</span>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li> -->

            <li>
              <router-link class="dropdown-item d-flex align-items-center" to="/login">
                <i class="bi bi-person"></i>
                <span>Protaille Etudiant</span>
              </router-link>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li>
              <router-link class="dropdown-item d-flex align-items-center" to="/login">
                <i class="bi bi-person"></i>
                <span>Portaille Aministratif</span>
              </router-link>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li>
              <router-link class="dropdown-item d-flex align-items-center" to="/login">
                <i class="bi bi-person"></i>
                <span>Autre Acces</span>
              </router-link>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <li>
              <a class="dropdown-item d-flex align-items-center" href="pages-faq.html">
                <i class="bi bi-question-circle"></i>
                <span>Bessoin d'aide?</span>
              </a>
            </li>
            <li>
              <hr class="dropdown-divider">
            </li>

            <!-- <li>
              <a class="dropdown-item d-flex align-items-center" href="#">
                <i class="bi bi-box-arrow-right"></i>
                <span>Sign Out</span>
              </a>
            </li> -->

          </ul><!-- End Profile Dropdown Items -->
          </li><!-- End Profile Nav -->
      </ul>
    </nav><!-- End Icons Navigation -->
</template>
<script>


export default {
  props:['ShowSearcheBar'],
  data(){
    return{
      connected:true,
    }
  },
  methods:{
    
  },
  onMounted(){
    console.log("bonsoir")
  }
  }
</script>
<style scoped>
</style>