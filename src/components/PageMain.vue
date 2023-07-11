<script>
import PageJumbo from './PageJumbo.vue';
import PageDescription from './PageDescription.vue';
import PageCard from './PageCard.vue'
export default {
    components: { PageJumbo, PageDescription, PageCard },
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
    </main>
</template>
<style scoped></style>