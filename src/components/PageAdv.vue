<script>
export default {
    data() {
        return {}
    }
}

</script>
<template>
    <section id="adv">
        <div class="container-fluid">
            <div class="row">
                <div class="col-6 p-0 d-flex text-center flex-column">
                    <h2>Get My Exclusive Investing Book just for $19.50</h2>
                    <p>Lorem ipsum, dolor sit amet consectetur adipisicing elit. Maxime consectetur reprehenderit voluptatem
                        corrupti cumque qui ullam.
                    </p>
                    <img class="partner" src="../assets/images/amazon.png" alt="">
                </div>
                <div class="col-5 d-flex justify-content-start align-items-end p-0">
                    <img class="book" src="../assets/images/book.png" alt="">
                </div>
                <div class="col-1 pe-0">
                    <div class="box d-flex flex-column text-center">
                        <i class="fa-solid fa-display"></i>
                        <i class="fa-solid fa-crosshairs"></i>
                        <i class="fa-solid fa-wrench"></i>
                        <i class="fa-solid fa-cart-shopping"></i>
                        <i class="fa-solid fa-mobile-screen-button"></i>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
#adv {
    background-image: url(../assets/images/slider_1-1917x607-1914x606.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

.row {
    height: 600px;
}

.book {
    height: 500px;
}

.partner {
    max-width: 230px;
    margin-top: 30px;
    margin-left: 355px;
    cursor: pointer;
}

h2 {
    color: #fcb900;
    font-size: 40px;
    padding-top: 130px;
    padding-left: 150px;
    padding-right: 60px;
}

p {
    color: white;
    font-size: 25px;
    padding-left: 150px;
    padding-right: 60px;
}

.box {
    background-color: white;
    width: 60px;
    height: 200px;
    margin-top: 150px;
    margin-left: 68px;
}

.fa-solid {
    margin: 12px auto;
    cursor: pointer;
}
</style>