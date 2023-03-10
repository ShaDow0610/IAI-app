<template>
    <div class="pagetitle">
        <nav>
            <ol class="breadcrumb">
            <li class="breadcrumb-item "><a href="index.html"><i class="bi bi-house fs-4"></i></a></li>
            <li class="breadcrumb-item fs-4">Components</li>
            <li class="breadcrumb-item active fs-4">Cards</li>
            </ol>
        </nav>
    </div><!-- End Page Title -->
    <headerFilter class=""/>


</template>
<script>
import headerFilter from '@/components/Layout/header/headerFilter.vue'
export default {
    components:{headerFilter},
    setup() {
        
    },
}
</script>