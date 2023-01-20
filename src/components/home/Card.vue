<template>
    <div class="col-lg-4 col-md-6 d-flex align-items-stretch mt-5" >
        <div class="course-item">
            <img src="@/assets/img/2.png" class="img-fluid " alt="..." >
            <div class="course-content">
                <div class="d-flex justify-content-between align-items-center mb-3">
                <h4>Classe</h4>
                <p class="time">02/03/2023<br/> 12h30</p>
            </div>
            <h3><router-link to="/postdetails">Sale de Classe</router-link></h3>
                <p>Et architecto provident deleniti facere repellat nobis iste. Id facere quia quae dolores dolorem tempore.</p>
                <div class="trainer d-flex justify-content-between align-items-center">
                    <div class="trainer-profile d-flex align-items-center">
                        <img src="@/assets/img/1.jpg" class="img-fluid" alt="">
                        <span>Paul Mibatket</span>
                    </div>
                    <div class="trainer-rank d-flex align-items-center">
                        <i class="bi bi-person text-success" ></i>&nbsp;{{ numffolowers }}
                        &nbsp;&nbsp;
                        <i class="like" @click="Likes" :class="[Clicked ? !Clicked:'bi bi-heart text-success','bi bi-heart-fill text-danger' ]"></i>&nbsp;{{ numlikes }}
                    </div>
                </div>
            </div>
        </div>
    </div> <!-- End Course Item-->
</template>
<script>
export default {
    data(){
        return{
            Clicked:false,
            numlikes:30,
            numffolowers:70,
        }
    },
    methods:{
        Likes(){
            this.Clicked=!this.Clicked;
            this.numlikes=this.numlikes+1;
        }
    }
}
</script>
<style scoped>
.courses .trainer .trainer-rank i:active{
  font-size:17px ;
}
.like:hover{
    cursor: pointer;
}


</style>