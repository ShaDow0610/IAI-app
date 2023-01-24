<template>
    <p>
          
    <button class="btn  position" type="button" data-bs-toggle="collapse" @click="tools" data-bs-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
        <i class="" :class="[!open ? close:'bi bi-chevron-double-right','bi bi-chevron-double-left']"></i>
    </button>
    </p>
    <div class="collapse" id="collapseExample">
        <Transition name="slide-fade">
            <div class="card card-body position2 p-0 mb-0 bg-secondary" v-if="show">
                <button class="btn btn-secondary fs-3 btn-lg m-2  p-0">
                    <i class="bi bi-plus-square"></i>
                </button>
                <button class="btn btn-secondary fs-4 btn-sm m-2  p-0">
                    <i class="bi bi-plus-square"></i>
                </button>
                <button class="btn btn-secondary fs-4 btn-sm m-2  p-0">
                    <i class="bi bi-plus-square"></i>
                </button>
                <button class="btn btn-secondary fs-4 btn-sm m-2  p-0">
                    <i class="bi bi-plus-square"></i>
                </button><button class="btn btn-secondary fs-4 btn-sm m-2  p-0">
                    <i class="bi bi-plus-square"></i>
                </button>
            </div>
        </Transition>
    </div>

</template>
<script>
export default {
    data(){
        return{
            open:false,
            show:false
        }
    },
    methods:{
        tools(){
            this.open=!this.open
            this.show=!this.show
        }
    }
}
</script>
<style scoped>
.position{
    position:fixed;
    top:122px;
    right:5px;
    color: black;
    background-color:green;

}
.position2{
    position:fixed;
    top:175px;
    right:5px;
    width: 60px;
}
/*
  Enter and leave animations can use different
  durations and timing functions.
*/
.slide-fade-enter-active {
  transition: all 0.3s ease-out;
}

.slide-fade-leave-active {
  transition: all 0.3s ease-in;
}

.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(20px);
  opacity: 0;
}

</style>