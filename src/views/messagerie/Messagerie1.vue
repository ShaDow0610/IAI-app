<template>  
    <main id="main" class="text-center">
        <MoptionBar/>
        <contacts/>
        <IBMessage/>
    </main>

</template>
<script>
import MoptionBar from '@/components/Layout/Messageries/MoptionBar.vue';
import contacts from '@/components/Layout/Messageries/contacts.vue'
import IBMessage from '@/components/Layout/Messageries/IBMessage.vue'
export default {
components:{MoptionBar,contacts,IBMessage},

}
</script>
<style scoped>
#main {
margin-top:0px !important;
padding: 0px;
}
</style>
