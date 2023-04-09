    <template>
        <headerB :ShowSideBar="ShowSideBar" :Toggeler="ToggleSideBar"/>
            
        <main id="main" class="text-center"  data-aos="fade-in" :class="[!this.ShowSideBar ? this.ShowSideBar:'responsive','responsive2']">
            <pageTitle ShowSideBar />
            <!-- ======= Breadcrumbs ======= -->
            <div class="breadcrumbs">
            <div class="container">
                <h2>BIENVENUE</h2>
                <p>ici nous vous presenton les publication les plus recente sur les activiter mener au sein de letblissement</p>
            </div>
            </div><!-- End Breadcrumbs -->
    
            <!-- ======= Courses Section ======= -->
            <section id="courses" class="courses main">
                <div class="container" data-aos="fade-up">
                    <div class="row d-flex justify-content-center " data-aos="zoom-in" data-aos-delay="100" >
                        <Card v-for="i in 50"/>
                    </div>
                </div>
                <COMELTools/>
            </section><!-- End Courses Section -->
    
        </main><!-- End #main -->
    </template>
    
    <script>
    
    import Card from '@/components/home/Card.vue';
    import pageTitle from '@/components/Layout/header/pageTitle.vue';
    import headerB from '@/components/Layout/header/headerB.vue';
    import COMELTools from '@/components/Layout/dashboardTools/COMELTools.vue';
    export default {
       components:{pageTitle,Card,headerB,COMELTools},
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
    <style>
    </style>
    
