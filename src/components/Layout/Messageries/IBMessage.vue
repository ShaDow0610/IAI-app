<template>
    <div class=" ib_m ">
        <div class="choose_person">
                <div class="text_p">
                    <div class="">
                        <div class="bi bi-chat-left"></div>
                        <div class="text">choose a person from your contacts tostart discussion</div>
                    </div>
                </div>
        </div>
        <div class="choose_personX">
            <div class="text_p">
                <div class="">
                    <div class="bi bi-chat-left"></div>
                    <div class="text">choose a person from your contacts tostart discussion</div>
                </div>
            </div>
    </div>
    </div>
</template>
<style scoped>
    .ib_m{
        background: black;
        color:white;
        position: fixed;
        right: 0;
        top: 0;
        bottom: 00;
        width: 62%;
        margin: 0;
    }
    .choose_person{

    }
    .text_p{
        position: fixed;
        top: 56%;
        left: 50%;
        color: white;
    }
    .text{
        width: 100%;
    }
    @media (max-width: 768px) {
        .ib_m{
            background: black;
            color:white;
            position: fixed;
            right: 0;
            top: 0;
            bottom: 00;
            width: 62%;
            margin: 0;
            display: none;
        }
        .choose_person{
    
        }
        .text_p{
            position: fixed;
            top: 56%;
            left: 50%;
            color: white;
        }
        .text{
            width: 100%;
        } 
    }
    .choose_personX{
        display: none;
        background: black;
        color:white;
        position: fixed;
        right: 0;
        top: 0;
        bottom: 00;
        width: 62%;
        margin: 0;
    }
</style>