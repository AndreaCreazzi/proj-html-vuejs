<script>
export default {
    props: {
        logoHeader: String,
        navbarOptions: Array
    },
    data() {
        return {
        }
    },
}
</script>
<template>
    <header>
        <nav class="container">
            <div class="row">
                <div class="col-6">
                    <img :src="`/src/assets/images/${logoHeader}`" alt="">
                </div>
                <div class="col-6 start">
                    <ul class="d-flex m-0 p-0 pe-5">
                        <p class="special">NEW</p>
                        <li class="list-unstyled mx-2" v-for="option in navbarOptions" :key="option.text"><a
                                :class="{ 'active': option.current }" :url="option.url">{{
                                    option.text }}</a></li>
                    </ul>
                    <i class="fa-brands fa-invision"></i>
                    <i class="fa-brands fa-instagram"></i>
                    <i class="fa-brands fa-facebook"></i>
                    <i class="fa-brands fa-twitter"></i>
                </div>
            </div>
        </nav>
    </header>
</template>
<style scoped>
.col-6 {
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
}

img {
    cursor: pointer;
}

.start {
    justify-content: start;
}

ul {
    position: relative;
}

.special {
    position: absolute;
    bottom: 0%;
    right: 36%;
    font-size: 7px;
    padding: 1px 5px;
    background-color: #dc1245;
    color: white;
    border-radius: 3px;
    font-weight: bold;
}

ul li a {
    text-decoration: none;
    color: black;
    padding-bottom: 0.5rem;
    font-weight: bold;
    cursor: pointer;
    transition: border-bottom 0.3s;
}

ul li a:hover,
.active {
    border-bottom: 2px solid #fcb900;
}

i:hover {
    color: #fcb900;
    cursor: pointer;
}

.fa-brands {
    margin: 0 5px;
    transition: color 0.5s;
}
</style>