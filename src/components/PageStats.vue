<script>
export default {
    data() {
        return {}
    }
}
</script>
<template>
    <section id="stats">
        <div class="container">
            <div class="row">
                <div class="col-3 d-flex justify-content-end align-items-center p-0">
                    <i class="fa-solid fa-user-group"></i>
                    <div class="d-flex flex-column">
                        <h3 class="m-0">3195</h3>
                        <p class="m-0">Online Learner</p>
                    </div>
                </div>
                <div class="col-3 d-flex justify-content-center align-items-center p-0">
                    <i class="fa-solid fa-clapperboard"></i>
                    <div class="d-flex flex-column">
                        <h3 class="m-0">23</h3>
                        <p class="m-0">Video Courses</p>
                    </div>
                </div>
                <div class="col-3 d-flex justify-content-center align-items-center p-0">
                    <i class="fa-sharp fa-solid fa-image"></i>
                    <div class="d-flex flex-column">
                        <h3 class="m-0">437</h3>
                        <p class="m-0">Sliders and Images</p>
                    </div>
                </div>
                <div class="col-3 d-flex justify-content-start align-items-center p-0">
                    <i class="fa-sharp fa-solid fa-thumbs-up"></i>
                    <div class="d-flex flex-column">
                        <h3 class="m-0">1140</h3>
                        <p class="m-0">Excellent Reviews</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
#stats {
    background-image: url(../assets/images/counter-1919x1101.jpg);
    background-size: cover;
}

.row {
    height: 500px;
}

.fa-solid {
    color: white;
    font-size: 50px;
    margin-right: 20px;
}

h3 {
    color: #fcb900;
}

p {
    color: white;
}
</style>