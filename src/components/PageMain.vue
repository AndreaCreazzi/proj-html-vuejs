<script>
import PageJumbo from './PageJumbo.vue';
import PageDescription from './PageDescription.vue';
import PageCard from './PageCard.vue'
import PageAdv from './PageAdv.vue';
import PageCourses from './PageCourses.vue'
import PageStats from './PageStats.vue';
export default {
    components: { PageJumbo, PageDescription, PageCard, PageAdv, PageCourses, PageStats },
    data() {
        return {}
    }
}
</script>
<template>
    <main>
        <!-- jumbotron -->
        <PageJumbo />
        <!-- section Description -->
        <PageDescription />
        <!-- section card -->
        <PageCard />
        <!-- section advertising -->
        <PageAdv />
        <!-- section courses -->
        <PageCourses />
        <!-- section stats -->
        <PageStats />
    </main>
</template>
<style scoped></style>