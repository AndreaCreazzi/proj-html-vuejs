<script>
export default {
    data() {
        return {}
    },
    props: {
        aboutInfo: Object,
        contactsInfo: Object,
        pagesInfo: Array,
        blogInfo: Array
    }
}
</script>
<template>
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-3">
                    <h3>ABOUT</h3>
                    <p class="about-first">{{ aboutInfo.site }}</p>
                    <p>{{ aboutInfo.company }}</p>
                    <p>{{ aboutInfo.developerCompany }}</p>
                    <div class="d-flex brands">
                        <i class="fa-brands fa-facebook"></i>
                        <i class="fa-brands fa-twitter"></i>
                        <i class="fa-brands fa-instagram"></i>
                    </div>
                </div>
                <div class="col-3">
                    <h3>CONTACT</h3>
                    <p class="contacts-first">{{ contactsInfo.place }}</p>
                    <p>{{ contactsInfo.phone }}</p>
                    <p>{{ contactsInfo.fax }}</p>
                    <p class="contacts-last">{{ contactsInfo.email }}</p>
                </div>
                <div class="col-3">
                    <h3>PAGES</h3>
                    <ul class="d-flex flex-wrap ps-3">
                        <li v-for="page in pagesInfo"><a>{{ page }}</a></li>
                    </ul>
                </div>
                <div class="col-3">
                    <h3>BLOG</h3>
                    <div v-for="blog in blogInfo" :key="blog.title" class="d-flex">
                        <img :src="`/src/assets/images/${blog.image}`" alt="">
                        <div class="d-flex flex-column right-description">
                            <h4>{{ blog.title }}</h4>
                            <p class="blockquote-footer">{{ blog.text }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </footer>
</template>
<style scoped>
footer {
    background-color: #fcb900;
}

.row {
    height: 500px;
}

h3 {
    padding-top: 70px;
    margin-bottom: 50px;
}

p {
    margin-bottom: 0;
}

.about-first {
    padding-right: 10px;
}

.brands {
    margin-top: 20px;
}

.fa-brands {
    margin-right: 20px;
    transition: color 0.5s;
    cursor: pointer;
}

.fa-brands:hover {
    color: white;
}

.contacts-first {
    margin-bottom: 20px;
    padding-right: 10px;
}

.contacts-last {
    margin-top: 20px;
}

ul li {
    flex-basis: calc(100% / 2);
    margin-bottom: 20px;
    transition: color 0.5s;
}

li:hover {
    color: white;
}

ul li a {
    cursor: pointer;
}

img {
    height: 80px;
    width: 80px;
    margin-bottom: 35px;
}

h4 {
    font-size: 15px;
    margin-bottom: 20px;
    padding-right: 70px;
    transition: color 0.5s;
    cursor: pointer;
}

h4:hover {
    color: white;
}

.right-description {
    margin-left: 10px;
}
</style>