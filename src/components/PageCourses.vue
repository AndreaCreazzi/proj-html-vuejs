<script>
export default {
    data() {
        return {}
    }
}
</script>
<template>
    <section id="courses">
        <h2 class="text-center py-5">Why my Courses?</h2>
        <div class="container">
            <div class="row">
                <div class="col-6 p-0 d-flex justify-content-center">
                    <div class="card mb-3" style="max-width: 540px;">
                        <div class="row g-0">
                            <div class="col-md-4 d-flex justify-content-center mt-5">
                                <i class="fa-sharp fa-solid fa-briefcase"></i>
                            </div>
                            <div class="col-md-8 d-flex justify-content-center mt-4">
                                <div class="card-body ps-0">
                                    <h5 class="card-title">Entrepreneurship</h5>
                                    <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum
                                        quibusdam quas corrupti velit consequatur ut recusandae doloremque veritatis, nihil
                                        mollitia neque incps-0idunt harem.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-6 p-0 d-flex justify-content-center">
                    <div class="card mb-3" style="max-width: 540px;">
                        <div class="row g-0">
                            <div class="col-md-4 d-flex justify-content-center mt-5">
                                <i class="fa-solid fa-rocket"></i>
                            </div>
                            <div class="col-md-8  d-flex justify-content-center mt-4">
                                <div class="card-body ps-0">
                                    <h5 class="card-title">Accelerated learning</h5>
                                    <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum
                                        quibusdam quas corrupti velit consequatur ut recusandae doloremque veritatis, nihil
                                        mollitia neque incidunt harem.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-6 p-0 d-flex justify-content-center">
                    <div class="card mb-3" style="max-width: 540px;">
                        <div class="row g-0">
                            <div class="col-md-4 d-flex justify-content-center mt-5">
                                <i class="fa-sharp fa-solid fa-thumbs-up"></i>
                            </div>
                            <div class="col-md-8  d-flex justify-content-center mt-4">
                                <div class="card-body ps-0">
                                    <h5 class="card-title">Productivity</h5>
                                    <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum
                                        quibusdam quas corrupti velit consequatur ut recusandae doloremque veritatis, nihil
                                        mollitia neque incidunt harem.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="col-6 p-0 d-flex justify-content-center">
                    <div class="card mb-3" style="max-width: 540px;">
                        <div class="row g-0">
                            <div class="col-md-4 d-flex justify-content-center mt-5">
                                <i class="fa-solid fa-gear"></i>
                            </div>
                            <div class="col-md-8  d-flex justify-content-center mt-4">
                                <div class="card-body ps-0">
                                    <h5 class="card-title">Life Coaching</h5>
                                    <p class="card-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum
                                        quibusdam quas corrupti velit consequatur ut recusandae doloremque veritatis, nihil
                                        mollitia neque incidunt harem.</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
.row {
    height: 700px;
}

h2 {
    font-size: 40px;
    font-weight: bold;
}

.card {
    height: 240px;
    border-left: 5px solid #fcb900;
    border-radius: 0%;
    cursor: pointer;
}

.fa-solid {
    font-size: 50px;
    color: #fcb900;
}

h5 {
    font-weight: bold;
    font-size: 25px;
}

.card:hover .fa-solid {
    color: white;
}

.card:hover {
    background-color: #fcb900;
}
</style>