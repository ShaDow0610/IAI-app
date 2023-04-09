<template>
<aside id="sidebar" class="sidebar  fade-right">

<ul class="sidebar-nav" id="sidebar-nav">

  <li class="nav-item">
    <a class="nav-link " href="index.html">
      <i class="bi bi-house"></i>
      <span>Acceuille</span>
    </a>
  </li><!-- End Dashboard Nav -->
  <li class="nav-item">
    <router-link to="/TimesTable" class="nav-link " >
      <i class="bi bi-calendar-week"></i>
      <span>Emplois du temps</span>
    </router-link>
  </li><!-- End Dashboard Nav -->
  <li class="nav-item">
    <router-link to="/cours" class="nav-link " >
      <i class="bi bi-book"></i>
      <span>Cours</span>
    </router-link>
  </li><!-- End Dashboard Nav -->
  <li class="nav-item">
    <router-link to="/devoi-expo" class="nav-link ">
      <i class="bi bi-book-half"></i>
      <span>Devoir & Exposer</span>
    </router-link>
  </li><!-- End Dashboard Nav -->
  <li class="nav-item">
    <a class="nav-link collapsed" data-bs-target="#components-nav" data-bs-toggle="collapse" href="#">
      <i class="bi bi-chat-dots"></i><span>Discussion</span><i class="bi bi-chevron-down ms-auto"></i>
    </a>
    <ul id="components-nav" class="nav-content collapse " data-bs-parent="#sidebar-nav">
      <li>
        <a href="components-alerts.html">
          <i class="bi bi-chat-left-text"></i><span>classe</span>
        </a>
      </li>
      <li>
        <a href="components-badges.html">
          <i class="bi bi-globe "></i><span>forum</span>
        </a>
      </li>
      <li>
        <a href="components-badges.html">
          <i class="bi bi-chat-square-text"></i><span>COMEL</span>
        </a>
      </li>
    </ul>
  </li><!-- End Components Nav -->
  <li class="nav-item">
    <a  class="nav-link collapsed" data-bs-target="#forms-nav" data-bs-toggle="collapse" href="#">
      <i class="bi bi-people"></i><span>Clubs</span><i class="bi bi-chevron-down ms-auto"></i>
    </a>
    <ul id="forms-nav" class="nav-content collapse " data-bs-parent="#sidebar-nav">
      <li>
        <router-link to="/clubHome">
          <i class="bi bi-circle"></i><span>Club 1</span>
        </router-link>
      </li>
      <li>
        <a href="forms-layouts.html">
          <i class="bi bi-circle"></i><span>Club 2</span>
        </a>
      </li>
      <li>
        <a href="forms-editors.html">
          <i class="bi bi-circle"></i><span>Club 3</span>
        </a>
      </li>
    </ul>
  </li><!-- End Forms Nav -->
  
 
  <li class="nav-item">
    <router-link to="/" class="nav-link " href="index.html">
      <i class="bi bi-grid"></i>
      <span>Comiter des Etudiant</span>
    </router-link>
  </li><!-- End Dashboard Nav -->
  <li class="nav-item">
    <router-link to="/delegueHome" class="nav-link ">
      <i class="bi bi-grid"></i>
      <span>Espace de Delegue</span>
    </router-link>
  </li><!-- End Dashboard Nav -->
  <li class="nav-item">
    <router-link to="/COMELHome" class="nav-link " href="index.html">
      <i class="bi bi-grid"></i>
      <span>COMEL</span>
    </router-link>
  </li><!-- End Dashboard Nav -->

  <li class="nav-item">
    <router-link to="/profile" class="nav-link collapsed" >
      <i class="bi bi-person"></i>
      <span>Profile</span>
    </router-link>
  </li><!-- End Profile Page Nav -->
  <li class="nav-item">
    <router-link to="/messagerie" class="nav-link collapsed">
      <i class="bi bi-envelope"></i>
      <span>Messagerie</span>
    </router-link>
  </li><!-- End Contact Page Nav -->

  <li class="nav-heading">Aministration</li>

 
  

  

  <li class="nav-item" v-if="!connected">
    <a class="nav-link collapsed" href="pages-login.html">
      <i class="bi bi-box-arrow-in-right"></i>
      <span>Login</span>
    </a>
  </li><!-- End Login Page Nav -->

  <li class="nav-item">
    <a class="nav-link collapsed" href="pages-error-404.html">
      <i class="bi bi-dash-circle"></i>
      <span>Scolariter</span>
    </a>
  </li><!-- End Error 404 Page Nav -->
  <li class="nav-item">
    <a class="nav-link collapsed" href="pages-register.html">
      <i class="bi bi-binoculars"></i>
      <span>Surveillance</span>
    </a>
  </li><!-- End Register Page Nav -->
  <li class="nav-item">
    <a class="nav-link collapsed" href="pages-blank.html">
      <i class="bi bi-cash-coin"></i>
      <span>Comptabiliter</span>
    </a>
  </li><!-- End Blank Page Nav -->
  
</ul>

</aside><!-- End Sidebar-->

</template>
<script>
export default {
    data(){
        return{
            connected:true,
        }
    }
    ,
    methods:{
         
    }
}
</script>
<style>
    
</style>