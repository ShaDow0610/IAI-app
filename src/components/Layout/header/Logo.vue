<template>
    <div class="d-flex align-items-center justify-content-between">
      <a href="index.html" class=" logo d-flex align-items-center ">
        <img  class="" src="@/assets/img/index.png"  alt="oppppsss">
        <div>
          <span class="d-lg-block ">
            <span class="color1">IAI</span>
            <span class="color2"> CAMEROUN</span>
          </span>
          <span class="d-none  d-lg-block fw-light fs-6 color3">Institus Africain d'Informatique</span>  
        </div>
      </a>
    </div><!-- End Logo -->
</template>
.<script>
export default {
  setup() {
    
  },
}
</script>
<style scoped>
.logo {
  line-height: 1;
}

@media (min-width: 1200px) {
  .logo {
    width: 50%;
  }
}

.logo img {
  max-height: 70px;
  margin-right:9px;
}

.logo span {
  font-size: 26px;
  font-weight: 700;
  /* color: #012970; */
  font-family: "Nunito", sans-serif;
}
.color1{
  color: green;
}
.color2{
  color: rgb(199, 171, 100);
}
.color3{
  color: black;
}
a{
  color:black;
  text-decoration: none repeat;

}

</style>
