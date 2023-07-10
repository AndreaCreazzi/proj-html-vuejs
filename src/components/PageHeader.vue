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
                    <ul class="d-flex m-0 p-0">
                        <li class="list-unstyled mx-2" v-for="option in navbarOptions" :key="option.text"><a
                                :class="{ 'active': option.current }" :url="option.url">{{
                                    option.text }}</a></li>
                    </ul>
                </div>
            </div>
        </nav>
    </header>
</template>
<style>
.col-6 {
    height: 100px;
    display: flex;
    justify-content: center;
    align-items: center;
}

.start {
    justify-content: start;
}

ul li a {
    text-decoration: none;
    color: black;
    padding-bottom: 0.5rem;
    font-weight: bold;
}

ul li a:hover,
.active {
    border-bottom: 2px solid #fcb900;
}
</style>