<script>
import PageJumbo from './PageJumbo.vue';
import PageDescription from './PageDescription.vue';
import PageCard from './PageCard.vue'
import PageAdv from './PageAdv.vue';
export default {
    components: { PageJumbo, PageDescription, PageCard, PageAdv },
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
    </main>
</template>
<style scoped></style>