<template>
    <!-- ======= Sidebar ======= -->
    <aside id="sidebar" class="sidebar">
        <ul class="sidebar-nav" id="sidebar-nav">
            <li class="nav-item">
                <a class="nav-link " href="index.html">
                <i class="bi bi-grid"></i>
                <span>Dashboard</span>
                </a>
            </li><!-- End Dashboard Nav -->
        </ul>
        <slot/>
    </aside><!-- End Sidebar-->
</template>
<script>
export default {
    methods:{
         
    }
}
</script>
<style>
     .sidebar {
        position: fixed;
        top: 80px;
        left: 0;
        bottom: 0;
        width: 300px;
        z-index: 996;
        transition: all 0.3s;
        padding: 20px;
        overflow-y: auto;
        scrollbar-width: thin;
        scrollbar-color: #aab7cf transparent;
        box-shadow: 0px 0px 20px rgba(1, 41, 112, 0.1);
        background-color: #fff;
    }
        @media (max-width: 1199px) {

        }

        .sidebar::-webkit-scrollbar {
        width: 5px;
        height: 8px;
        background-color: #fff;
        }

        .sidebar::-webkit-scrollbar-thumb {
        background-color: #aab7cf;
        }

</style>