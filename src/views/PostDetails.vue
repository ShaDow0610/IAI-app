<template>
     <headerB :ShowSideBar="ShowSideBar" :Toggeler="ToggleSideBar"/>
    <main id="main" class=""  data-aos="fade-in" :class="[!ShowSideBar ? ShowSideBar:'responsive','responsive2']">

        <!-- ======= Breadcrumbs ======= -->
        <div class="breadcrumbs" data-aos="fade-in">
        <div class="container">
            <h2>Details de la publication</h2>
            <p>Est dolours ut non facere possimus quibusdam eligendi voluptatem. Quia id aut similique quia voluptas sit quaerat debitis. Rerum omnis ipsam aperiam consequatur laboriosam nemo harum praesentium. </p>
        </div>
        </div><!-- End Breadcrumbs -->

        <!-- ======= Cource Details Section ======= -->
        <section id="course-details" class="course-details">
        <div class="container" data-aos="fade-up">

            <div class="row">
            <div class="col-lg-8">
                <img src="@/assets/img/BreakingBad2.png" class="img-fluid" alt="">
                <h3>Et enim incidunt fuga tempora</h3>
                <p>
                Qui et explicabo voluptatetastem et ab qui vero et voluptas. Sint voluptates temporibus quam autem. Atque nostrum voluptatum laudantium a doloremque enim et ut dicta. Nostrum ducimus est iure minima totam doloribus nisi ullam deserunt. Corporis aut officiis sit nihil est. Labore aut sapiente aperiam.
                Qui voluptas qui vero ipsum ea voluptatem. Omnis et est. Voluptatem officia voluptatem adipisci et iusto provident doloremque consequatur. Quia et porro est. Et qui corrupti laudantium ipsa.
                Eum quasi saepe aperiam qui delectus quaerat in. Vitae mollitia ipsa quam. Ipsa aut qui numquam eum iste est dolorum. Rem voluptas ut sit ut.
                </p>
            </div>
            <div class="col-lg-4">

                <div class="course-info d-flex justify-content-between align-items-center">
                <h5>Publier par</h5>
                <p><a href="#">Walter White</a></p>
                </div>

                <div class="course-info d-flex justify-content-between align-items-center">
                <h5>C</h5>
                <p>$165</p>
                </div>

                <div class="course-info d-flex justify-content-between align-items-center">
                <h5>Available Seats</h5>
                <p>30</p>
                </div>

                <div class="course-info d-flex justify-content-between align-items-center">
                <h5>Heure de publication</h5>
                <p>5.00 pm - 7.00 pm</p>
                </div>

            </div>
            </div>

        </div>
        </section><!-- End Cource Details Section -->

        <!-- ======= Cource Details Tabs Section ======= -->
        <section id="cource-details-tabs" class="cource-details-tabs">
        <div class="container" data-aos="fade-up">

            <div class="row">
            <div class="col-lg-3">
                <ul class="nav nav-tabs flex-column">
                <li class="nav-item">
                    <a class="nav-link active show" data-bs-toggle="tab" href="#tab-1">Publier par</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" data-bs-toggle="tab" href="#tab-2">Porté</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" data-bs-toggle="tab" href="#tab-3">Pariatur explicabo vel</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" data-bs-toggle="tab" href="#tab-4">Collection d'image</a>
                </li>
                <li class="nav-item">
                    <a class="nav-link" data-bs-toggle="tab" href="#tab-5">Heure de publicationt</a>
                </li>
                </ul>
            </div>
            <div class="col-lg-9 mt-4 mt-lg-0">
                <div class="tab-content">
                <div class="tab-pane active show" id="tab-1">
                    <div class="row">
                    <div class="col-lg-8 details order-2 order-lg-1">
                        <h3>cette Publication a ete effectuer par</h3>
                        <p class="fst-italic">Qui laudantium consequatur laborum sit qui ad sapiente dila parde sonata raqer a videna mareta paulona marka</p>
                        <p>Et nobis maiores eius. Voluptatibus ut enim blanditiis atque harum sint. Laborum eos ipsum ipsa odit magni. Incidunt hic ut molestiae aut qui. Est repellat minima eveniet eius et quis magni nihil. Consequatur dolorem quaerat quos qui similique accusamus nostrum rem vero</p>
                    </div>
                    <div class="col-lg-4 text-center order-1 order-lg-2">
                        <img src="assets/img/course-details-tab-1.png" alt="" class="img-fluid">
                    </div>
                    </div>
                </div>
                <div class="tab-pane" id="tab-2">
                    <div class="row">
                    <div class="col-lg-8 details order-2 order-lg-1">
                        <h3>Et blanditiis nemo veritatis excepturi</h3>
                        <p class="fst-italic">Qui laudantium consequatur laborum sit qui ad sapiente dila parde sonata raqer a videna mareta paulona marka</p>
                        <p>Ea ipsum voluptatem consequatur quis est. Illum error ullam omnis quia et reiciendis sunt sunt est. Non aliquid repellendus itaque accusamus eius et velit ipsa voluptates. Optio nesciunt eaque beatae accusamus lerode pakto madirna desera vafle de nideran pal</p>
                    </div>
                    <div class="col-lg-4 text-center order-1 order-lg-2">
                        <img src="assets/img/course-details-tab-2.png" alt="" class="img-fluid">
                    </div>
                    </div>
                </div>
                <div class="tab-pane" id="tab-3">
                    <div class="row">
                    <div class="col-lg-8 details order-2 order-lg-1">
                        <h3>Impedit facilis occaecati odio neque aperiam sit</h3>
                        <p class="fst-italic">Eos voluptatibus quo. Odio similique illum id quidem non enim fuga. Qui natus non sunt dicta dolor et. In asperiores velit quaerat perferendis aut</p>
                        <p>Iure officiis odit rerum. Harum sequi eum illum corrupti culpa veritatis quisquam. Neque necessitatibus illo rerum eum ut. Commodi ipsam minima molestiae sed laboriosam a iste odio. Earum odit nesciunt fugiat sit ullam. Soluta et harum voluptatem optio quae</p>
                    </div>
                    <div class="col-lg-4 text-center order-1 order-lg-2">
                        <img src="assets/img/course-details-tab-3.png" alt="" class="img-fluid">
                    </div>
                    </div>
                </div>
                <div class="tab-pane" id="tab-4">
                    <div class="row">
                    <div class="col-lg-8 details order-2 order-lg-1">
                        <h3>Fuga dolores inventore laboriosam ut est accusamus laboriosam dolore</h3>
                        <p class="fst-italic">Totam aperiam accusamus. Repellat consequuntur iure voluptas iure porro quis delectus</p>
                        <p>Eaque consequuntur consequuntur libero expedita in voluptas. Nostrum ipsam necessitatibus aliquam fugiat debitis quis velit. Eum ex maxime error in consequatur corporis atque. Eligendi asperiores sed qui veritatis aperiam quia a laborum inventore</p>
                    </div>
                    <div class="col-lg-4 text-center order-1 order-lg-2">
                        <img src="assets/img/course-details-tab-4.png" alt="" class="img-fluid">
                    </div>
                    </div>
                </div>
                <div class="tab-pane" id="tab-5">
                    <div class="row">
                    <div class="col-lg-8 details order-2 order-lg-1">
                        <h3>Details sur l'heure ou la publication a effectuer</h3>
                        <p class="fst-italic">Omnis blanditiis saepe eos autem qui sunt debitis porro quia.</p>
                        <p>Exercitationem nostrum omnis. Ut reiciendis repudiandae minus. Omnis recusandae ut non quam ut quod eius qui. Ipsum quia odit vero atque qui quibusdam amet. Occaecati sed est sint aut vitae molestiae voluptate vel</p>
                    </div>
                    <div class="col-lg-4 text-center order-1 order-lg-2">
                        <img src="assets/img/course-details-tab-5.png" alt="" class="img-fluid">
                    </div>
                    </div>
                </div>
                </div>
            </div>
            </div>

        </div>
        </section><!-- End Cource Details Tabs Section -->

        </main><!-- End #main -->

</template>

<script>
import Card from '@/components/home/Card.vue';
import pageTitle from '@/components/Layout/header/pageTitle.vue';
import headerB from '@/components/Layout/header/headerB.vue';

export default {
   components:{pageTitle,Card,headerB},
   data(){
    return{
        ShowSideBar:false,
    }
   },
  methods:{
    ToggleSideBar(){
            this.ShowSideBar=!this.ShowSideBar
            
        },

  }
}
</script>
<style scoped>
.responsive{
    margin-left: 300px;
    transition: 0.7s;
} 
.responsive2{
 
    transition: 0.9s;
}
    .course-details h3 {
  font-size: 24px;
  margin: 30px 0 15px 0;
  font-weight: 700;
  position: relative;
  padding-bottom: 10px;
}

.course-details h3:before {
  content: "";
  position: absolute;
  display: block;
  width: 100%;
  height: 1px;
  background: #eef0ef;
  bottom: 0;
  left: 0;
}

.course-details h3:after {
  content: "";
  position: absolute;
  display: block;
  width: 60px;
  height: 1px;
  background: #5fcf80;
  bottom: 0;
  left: 0;
}

.course-details .course-info {
  background: #f6f7f6;
  padding: 10px 15px;
  margin-bottom: 15px;
}

.course-details .course-info h5 {
  font-weight: 400;
  font-size: 16px;
  margin: 0;
  font-family: "Poppins", sans-serif;
}

.course-details .course-info p {
  margin: 0;
  font-weight: 600;
}

.course-details .course-info a {
  color: #657a6d;
}
/*--------------------------------------------------------------
# Cource Details Tabs
--------------------------------------------------------------*/
.cource-details-tabs {
  overflow: hidden;
  padding-top: 0;
}

.cource-details-tabs .nav-tabs {
  border: 0;
}

.cource-details-tabs .nav-link {
  border: 0;
  padding: 12px 15px 12px 0;
  transition: 0.3s;
  color: #37423b;
  border-radius: 0;
  border-right: 2px solid #e2e7e4;
  font-weight: 600;
  font-size: 15px;
}

.cource-details-tabs .nav-link:hover {
  color: #5fcf80;
}

.cource-details-tabs .nav-link.active {
  color: #5fcf80;
  border-color: #5fcf80;
}

.cource-details-tabs .tab-pane.active {
  -webkit-animation: fadeIn 0.5s ease-out;
  animation: fadeIn 0.5s ease-out;
}

.cource-details-tabs .details h3 {
  font-size: 26px;
  font-weight: 600;
  margin-bottom: 20px;
  color: #37423b;
}

.cource-details-tabs .details p {
  color: #777777;
}

.cource-details-tabs .details p:last-child {
  margin-bottom: 0;
}

@media (max-width: 992px) {
  .cource-details-tabs .nav-link {
    border: 0;
    padding: 15px;
  }

  .cource-details-tabs .nav-link.active {
    color: #fff;
    background: #5fcf80;
  }
}

</style>