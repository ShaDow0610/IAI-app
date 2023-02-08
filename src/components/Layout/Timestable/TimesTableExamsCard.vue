<template>
    <!-- Card with an image on top -->
    <div class="card">
        <img src="assets/img/card.jpg" class="card-img-top" alt="...">
        <div class="card-body">
            <table class="table">
                <thead>
                    <tr>
                    
                    <th scope="col">heure</th>
                    <th scope="col">jours</th>
                    <th scope="col">matiere</th>
                    </tr>
                </thead>
                <tbody>
                    <tr v-for="i in 80">
                        <td>Mark</td>
                        <td>Otto</td>
                        <td>@mdo</td>
                    </tr>
                </tbody>
                </table>
        </div>
    </div><!-- End Card with an image on top -->
</template>