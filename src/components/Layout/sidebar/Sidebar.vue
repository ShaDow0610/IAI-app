<template>
<aside id="sidebar" class="sidebar">

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
    <a class="nav-link " href="index.html">
      <i class="bi bi-book-half"></i>
      <span>Devoir & Exposer</span>
    </a>
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
        <router-link to="/ClubJournal">
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
    <router-link to="/" class="nav-link " href="index.html">
      <i class="bi bi-grid"></i>
      <span>Espace de Delegue</span>
    </router-link>
  </li><!-- End Dashboard Nav -->
  <li class="nav-item">
    <router-link to="/" class="nav-link " href="index.html">
      <i class="bi bi-grid"></i>
      <span>Espace de sous Delegue</span>
    </router-link>
  </li><!-- End Dashboard Nav -->

  <li class="nav-item">
    <a class="nav-link collapsed" href="users-profile.html">
      <i class="bi bi-person"></i>
      <span>Profile</span>
    </a>
  </li><!-- End Profile Page Nav -->
  <li class="nav-item">
    <a class="nav-link collapsed" href="pages-contact.html">
      <i class="bi bi-envelope"></i>
      <span>Messagerie</span>
    </a>
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
      a{
        text-decoration: none !important;
      }
     .sidebar {
        position: fixed;
        top: 120px;
        left: 0;
        bottom: 0;
        width: 300px;
        z-index: 996;
        transition: all 0.3s;
        padding: 20px;
        overflow-y: auto;
        scrollbar-width: thin;
        scrollbar-color: #aab7cf transparent;
        box-shadow: 0px 0px 20px rgba(1, 41, 112, 0.1);
        background-color: #fff;
    }
    @media (max-width: 1199px) {

        }

        .sidebar::-webkit-scrollbar {
        width: 5px;
        height: 8px;
        background-color: #fff;
        }

        .sidebar::-webkit-scrollbar-thumb {
        background-color: #aab7cf;
        }
        /* @media (min-width: 1200px) {

        #main,
        #footer {
        margin-left: 300px;
        }
        } */

        @media (max-width: 1199px) {
        .toggle-sidebar .sidebar {
        left: 0;
        }
        }

        @media (min-width: 1200px) {

        .toggle-sidebar #main,
        .toggle-sidebar #footer {
        margin-left: 0;
        }

        .toggle-sidebar .sidebar {
        left: -300px;
        }
        }

        .sidebar-nav {
        padding: 0;
        margin: 0;
        list-style: none;
        }

        .sidebar-nav li {
        padding: 0;
        margin: 0;
        list-style: none;
        }

        .sidebar-nav .nav-item {
        margin-bottom: 5px;
        }

        .sidebar-nav .nav-heading {
        font-size: 11px;
        text-transform: uppercase;
        color: green;
        font-weight: 600;
        margin: 10px 0 5px 15px;
        }

        .sidebar-nav .nav-link {
        display: flex;
        align-items: center;
        font-size: 15px;
        font-weight: 600;
        color: black;
        transition: 0.3;
        background: #fffcf6;
        padding: 10px 15px;
        border-radius: 4px;
        }

        .sidebar-nav .nav-link i {
        font-size: 16px;
        margin-right: 10px;
        color:rgb(199, 171, 100);
        }

        .sidebar-nav .nav-link.collapsed {
        color: black;
        background: #fffcf6;
        }

        .sidebar-nav .nav-link.collapsed i {
        color: rgb(199, 171, 100);
        }

        .sidebar-nav .nav-link:hover {
        color: rgb(28, 29, 28);
        background: #f6fff6;
        font-size: 16px;
        }

        .sidebar-nav .nav-link:hover i {
        color: green;
        }
        .sidebar-nav .nav-link:active i {
        color: green;
        }

        .sidebar-nav .nav-link .bi-chevron-down {
        margin-right: 0;
        transition: transform 0.2s ease-in-out;
        }

        .sidebar-nav .nav-link:not(.collapsed) .bi-chevron-down {
        transform: rotate(180deg);
        }

        .sidebar-nav .nav-content {
        padding: 5px 0 0 0;
        margin: 0;
        list-style: none;
        }

        .sidebar-nav .nav-content a {
        display: flex;
        align-items: center;
        font-size: 14px;
        font-weight: 600;
        color: black;
        transition: 0.3;
        padding: 10px 0 10px 40px;
        transition: 0.3s;
        }

        .sidebar-nav .nav-content a i {
        font-size: 15px;
        margin-right: 8px;
        line-height: 0;
        border-radius: 50%;
        }

        .sidebar-nav .nav-content a:hover,
        .sidebar-nav .nav-content a.active {
        color: green;
        background: #f6fff6;

        }

        .sidebar-nav .nav-content a.active i {
        background-color: green;
        background: #f6fff6;
        }

</style>