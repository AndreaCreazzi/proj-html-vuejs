<script>
import PageHeader from './components/PageHeader.vue';
import PageMain from './components/PageMain.vue';
import PageFooter from './components/PageFooter.vue';
export default {
  components: { PageHeader, PageMain, PageFooter },
  data() {
    return {
      logoHeader: "MasterStudy-1.svg",
      navbarOptions: [
        {
          text: 'Courses',
          url: '#',
          current: false,
        },
        {
          text: 'Courses Format',
          url: '#',
          current: false,
        },
        {
          text: 'Add Courses',
          url: '#',
          current: false,
        },
        {
          text: 'Pages',
          url: '#',
          current: false,
        },
        {
          text: 'Demos',
          url: '#',
          current: true,
        }
      ]
    }
  }
}
</script>
<template>
  <PageHeader :logoHeader="logoHeader" :navbarOptions="navbarOptions" />
  <PageMain />
  <PageFooter />
</template>
<style></style>