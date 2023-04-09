<template>
    <div class="MessageContainer">
        <img src="logo.png" alt="Logo">
        <div class="input-group mt-3 rounded">
            <input type="text" class="form-control" placeholder="Recherche">
            <button class="btn message-input-group-addon "><i class="bi bi-search"></i></button>
        </div>
        <div class="messages mt-4">
            <div class="message-block rounded" data-conversation="conversation1">
                <img src="profile1.jpg" alt="Profil">
                <p>Message 1</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <!-- Ajouter les autres blocs de message ici -->
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            <div class="message-block">
                <img src="profile2.jpg" alt="Profil">
                <p>Message 2</p>
                <span>Heure d'envoi</span>
            </div>
            

            
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scooped>
.MessageContainer {
width: 30%;
position: fixed;
left: 8%;
top: 0;
bottom: 0;
background: rgb(26, 26, 26);
color:white;
max-width: 720px;
padding-right: var(--bs-gutter-x,.75rem);
padding-left: var(--bs-gutter-x,.75rem);
margin-right: auto;
margin-left: auto;

}

.message-block {
    background-color: #313131;
    margin-bottom: 10px;
    padding: 10px;
    border-radius: 10px;

}
.message-block:nth-child(odd) {
    background-color: #313131;
}
.message-input-group-addon{
    color:black;
    background-color: white;
}
.messages{
    overflow-y: auto;
    scrollbar-width: none;
}
@media (max-width: 768px) {
    .MessageContainer {
        width: 100%;
        position: fixed;
        max-width: unset;
        padding-bottom: 45px;
        left: 0;       
    }
    .messages{
        overflow-y: auto;
        scrollbar-width: none;
    }
    .message-input-group-addon{
        color:black;
        background-color: white;
        
    }
}
</style>