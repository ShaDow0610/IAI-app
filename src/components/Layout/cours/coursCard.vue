<template>
    <div class="col-lg-6 offset-lg-3">
        <div class="card">
          <div class="card-body">
            <h5 class="card-title">Cours de cette semaine</h5>

            <!-- Accordion without outline borders -->
            <div class="accordion accordion-flush" id="accordionFlushExample">
              <Cours/>
              <Cours/>
              <Cours/>
              <Cours/>
              <Cours/>
            </div><!-- End Accordion without outline borders -->

          </div>
        </div>

      </div>
</template>
<script>
import Cours from "@/components/Layout/cours/Cours.vue"
export default {
  components:{Cours}
}
</script>
