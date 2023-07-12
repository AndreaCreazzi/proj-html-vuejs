<script>
export default {
    data() {
        return {
            email: '',
            arrEmail: [],
            seconds: 60,
            minutes: 47
        }
    },
    mounted() {
        this.startTimer();
    },
    methods: {
        emailGet() {
            this.arrEmail.push(this.email)
            this.email = '';
        },
        startTimer() {
            setInterval(() => {
                this.seconds--;
                if (this.seconds === 0) {
                    this.seconds = 60;
                    this.minutes--;
                }
            }, 1000);
        }
    }
}
</script>
<template>
    <section id="jumbotron">
        <div class="container">
            <div class="row">
                <div id="up" class="col-12 d-flex justify-content-center align-items-center flex-column">
                    <h1 class="m-0">Start your Human <strong class="subcolor-y">Revolution</strong> today</h1>
                    <p class="text">A wonderful serenity has taken possession of my entire soul, like these sweet
                        mornings of spring
                        which i enjoy with my whole heart.</p>
                </div>
                <div id="bottom" class="col-12">
                    <div class="row main">
                        <div class="col-6 d-flex justify-content-center flex-column">
                            <h4 class="ps-5 mb-3"><strong class="subcolor-w">Limited Sale:</strong> All courses with 55%
                                off
                            </h4>
                            <div class="input-group px-5">
                                <input v-model="email" type="email" class="form-control py-2"
                                    placeholder="Enter your E-mail" @keyup.enter="emailGet">
                                <button @click="emailGet" type="button">Subscribe</button>
                            </div>
                        </div>
                        <div class="col-6">
                            <div class="row main ">
                                <div class="col-3">
                                    <h2>26</h2>
                                    <h5>Days</h5>
                                </div>
                                <div class="col-3">
                                    <h2>01</h2>
                                    <h5>Hours</h5>
                                </div>
                                <div class="col-3">
                                    <h2>{{ minutes }}</h2>
                                    <h5>Minutes</h5>
                                </div>
                                <div class="col-3">
                                    <h2>{{ seconds }}</h2>
                                    <h5>Seconds</h5>
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
#jumbotron {
    height: 650px;
    background-image: url(../assets/images/slide-1.jpg);
    background-repeat: no-repeat;
    background-size: cover;
}

#up {
    height: 425px;
}

#bottom {
    margin-top: 100px;
    padding: 0 100px;
}

#bottom,
.main {
    height: 200px;
}

.col-6 {
    background-color: #fcb900;
}

.col-3 {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
}

h1 {
    padding-top: 150px;
    padding-left: 525px;
    padding-right: 250px;
    font-weight: bold;
    font-size: 60px;
}

h4 {
    font-weight: bold;
}

h2 {
    color: white;
    font-size: 60px;
}

.subcolor-y {
    color: #fcb900;
}

.subcolor-w {
    color: white;
}

.text {
    padding-left: 525px;
    padding-right: 300px;
    margin-bottom: 0;
    margin-top: 15px;
}

input {
    border-radius: 50px;
}

button {
    border-radius: 50px;
    background-color: #2d4649;
    color: white;
    padding: 10px;
}
</style>