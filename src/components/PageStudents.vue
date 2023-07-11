<script>
export default {
    data() {
        return {
            autoPlay: null,
            // index corrente
            currentIndex: 0,
            // array di oggetti
            students: [
                {
                    image: '/src/assets/images/1-100x100.jpg',
                    title: 'Come as you are',
                    text: 'MasterStudy used is an excellent workshop whether you come as a counselor, advisor, administrator, or faculty member. I am going home empowered. I am looking forward to attending the On Course MasterStudy and the MasterStudy National Conference next year and facilitating the use of this excellent retention/student success course at my college.',
                },
                {
                    image: '/src/assets/images//2-100x100.jpg',
                    title: 'Paints of the Future',
                    text: 'The response to your MasterStudy has been really overwhelming! Those who participated in the workshop are spreading the word here on campus and the “buzz” is on. The VP of Instruction wants you to come back! Her goal is to have more faculty trained. She also wants to attend a workshop herself. Our President told me Masterstudy needs to be the cornerstone of our success program.',
                },
                {
                    image: '/src/assets/images/4-100x100.jpg',
                    title: 'Investing for Your Future',
                    text: "It is no exaggeration to say this MasterStudy experience was transformative both professionally and personally. This workshop will long remain a high point of my life. Thanks again…. I am feeling energized and eager to start teaching my class next week. I can’t wait to use all of my new teaching tools. I will absolutely recommend this workshop to other educators!",
                },
            ],
        }
    },
    computed: {
        lastIndex() {
            return this.students.length - 1;
        },
        isLastImage() {
            return this.currentIndex == this.lastIndex;
        }
    },
    methods: {
        goToNext() {
            if (this.isLastImage) this.currentIndex = 0;
            else this.currentIndex++;
        },
        goToPrev() {
            if (this.currentIndex) this.currentIndex--;
            else this.currentIndex = this.lastIndex;
        },
        setCurrentIndex(targetIndex) {
            this.currentIndex = targetIndex;
        },
        stopAutoPlay() {
            clearInterval(this.autoPlay);
        },
        startAutoPlay() {
            this.autoPlay = setInterval(this.goToNext, 4000);
        }
    },
    mounted() {
        this.startAutoPlay()
    }
}
</script>
<template>
    <section id="students">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <h2 class="text-center py-5">What Students Say</h2>
                    <div class="d-flex justify-content-center">
                        <!-- tasto prev -->
                        <!-- galleria -->
                        <div class="d-flex justify-content-center">
                            <i class="fa-solid fa-arrow-left mt-4" id="prev" @click="goToPrev" @mouseenter="stopAutoPlay"
                                @mouseleave="startAutoPlay"></i>
                            <figure v-for="(student, i) in students">
                                <div class="d-flex justify-content-center align-items-center">
                                    <img :src="student.image" :alt="student.text" :title="student.title">
                                </div>
                                <figcaption>
                                    <div class="d-flex justify-content-center align-items-center flex-column">
                                        <strong v-show="currentIndex === i" class=" text-center">{{ student.title
                                        }}</strong>
                                        <div v-show="currentIndex === i">
                                            <i class="fa-solid fa-star"></i>
                                            <i class="fa-solid fa-star"></i>
                                            <i class="fa-solid fa-star"></i>
                                            <i class="fa-solid fa-star"></i>
                                            <i class="fa-solid fa-star"></i>
                                        </div>
                                        <p class="text-center" v-show="currentIndex === i">{{ student.text }}</p>
                                    </div>
                                </figcaption>
                            </figure>
                            <i class="fa-solid fa-arrow-right mt-4" id="prev" @click="goToNext" @mouseenter="stopAutoPlay"
                                @mouseleave="startAutoPlay"></i>
                        </div>
                        <!-- testo next -->
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
.row {
    height: 600px;
}

h2 {
    font-size: 40px;
    font-weight: bold;
}


img {
    border-radius: 50px;
    margin-left: 100px;
    margin-right: 100px;
    margin-bottom: 10px;
}

.fa-arrow-left,
.fa-arrow-right {
    font-size: 30px;
}

.fa-star {
    color: #fcb900;
    margin-bottom: 30px;
}

strong {
    font-size: 20px;
}
</style>