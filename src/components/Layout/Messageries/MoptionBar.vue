<template>
    <div class="MessageToolBar">
        <button class="btn btn-primary  p-0 logo_btn ">
          <router-link to="/">
              <img src="logo.png " alt="Logo" class="logo ">
          </router-link>
        </button>
        <button class="btn btn-primary"><i class="bi bi-person"></i><span> Personne</span></button>
        <button class="btn btn-primary"><i class="bi bi-chat-left-text"></i><span> Message</span></button>
        <button class="btn btn-primary"><i class="bi bi-plus"></i><span> Plus</span></button>
        <button class="btn btn-primary"><i class="bi bi-bell"></i><span> Cloche</span></button>
        <button class="btn btn-primary"><i class="bi bi-gear"></i><span> Paramètre</span></button>
      </div>
</template>
<style scoped>
.MessageToolBar {
    position: fixed;
    left: 0;
    top: 0;
    width: 8%;
    height: 100%;
    transition: width 0.5s;
    background: black;
    padding: 10px;
    bottom: 0;
    z-index: 996;
    overflow-y: auto;
    scrollbar-width: thin;
    scrollbar-color: #1b1b1b transparent;
    box-shadow: 0px 0px 20px rgba(1, 41, 112, 0.1);
        
  }

  .MessageToolBar:hover {
    width: 15%;
    
  }

 .logo_btn{
  margin-bottom: 125px !important;
  border:none
 }
  .logo {
    display: block;
    max-width: 100%;
    background-color: black; 
  }

  .MessageToolBar button {
    display: block;
    width: 100%;
    padding: auto ;
    margin-top: 20px;
    margin-bottom: 20px;
    margin-right:10px ;
    background-color: rgb(24, 24, 24);
    border-color: rgb(24, 24, 24);
    margin-bottom: 45px;
  }
  .MessageToolBar button:hover {
    
    background-color: rgb(48, 48, 48);
    border-color: rgb(48, 48, 48);
  }
  
  .MessageToolBar:hover button span {
    display:inline;
    
  }
  
  .MessageToolBar button span {
    display:none;
  }
  
  @media (max-width: 768px) {
    .MessageToolBar {
      position: fixed;
      bottom: 0;
      left: 0;
      width: 100% !important;
      height: 45px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 10px;
      top: unset;
      transition: none;
    }
    .MessageToolBar:hover button span {
    display:none !important;
  }
  .MessageToolBar button span {
    display:none !important;
  }
    
    .MessageToolBar button {
    display: block;
    width: 50%;
    margin-bottom: 20px;
    
  }
    .logo {
      display:none !important;
    }
  }
</style>