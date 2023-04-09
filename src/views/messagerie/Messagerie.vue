<template>
        <main id="main" class="text-center" >
            <Messagerie/>
        </main>
</template>
<script>

import Messagerie from '@/components/Layout/Messageries/Messagerie.vue';

export default {
   components:{Messagerie},
}
</script>
<style scoped>
#main {
    margin-top:0px !important;
    padding: 0px;
  }
</style>