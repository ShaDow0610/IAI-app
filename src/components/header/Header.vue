<template>
    <header id="header" class="header fixed-top d-flex align-items-center">
       <slot/>
    </header>
</template>
<script>


export default ({
    name: 'Header',
    components:{ },
    setup() {
        
    },
})
</script>
<style scoped>

.header {
  transition: all 0.5s;
  z-index: 997;
  height: 80px;
  box-shadow: 0px 2px 20px rgba(1, 41, 112, 0.1);
  background-color: #fff;
  padding-left: 20px;
  /* Toggle Sidebar Button */
  /* Search Bar */
}

@media(max-width: 1199px) {
    .header{
        background: black;
    }
}
@media(min-width: 1200px) {
    .header{
        background: rgb(132, 35, 35);
    }
}
</style>
