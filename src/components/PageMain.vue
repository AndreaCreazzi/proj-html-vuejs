<script>
import PageJumbo from './PageJumbo.vue';
import PageDescription from './PageDescription.vue';
import PageCard from './PageCard.vue'
import PageAdv from './PageAdv.vue';
import PageCourses from './PageCourses.vue'
import PageStats from './PageStats.vue';
import PageStudents from './PageStudents.vue';
export default {
    components: { PageJumbo, PageDescription, PageCard, PageAdv, PageCourses, PageStats, PageStudents },
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
        <!-- section students -->
        <PageStudents />
    </main>
</template>
<style scoped></style>