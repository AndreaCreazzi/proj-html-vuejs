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
      ],
      aboutInfo: {
        site: 'Masterstudy is Education WordPress theme featured by Learning.',
        company: 'Management System (LMS) for online education',
        developerCompany: 'Developed by StylemixThemes'
      },
      contactsInfo: {
        place: 'USA, Callifornia 20, First Avenue, Callifornia',
        phone: '+1 212 458 300 32',
        fax: '+1 212 375 24 14',
        email: 'info@masterstudy.com'
      },
      pagesInfo: ['blog', 'Courses', 'Home', 'Membership A..', 'Shortcodes', 'Typography'],
      blogInfo: [
        {
          image: 'photo-1517520287167-4bbf64a00d66-150x150.jpeg',
          title: 'Our main target is to "Developing Yourself as a Leader"',
          text: 'August 9, 2018'
        },
        {
          image: 'photo-1490376840453-5f616fbebe5b-150x150.jpeg',
          title: 'Those Other College Expenses You Are Not Thinking About',
          text: 'June 3, 2015'
        }
      ]
    }
  }
}
</script>
<template>
  <PageHeader :logoHeader="logoHeader" :navbarOptions="navbarOptions" />
  <PageMain />
  <PageFooter :aboutInfo="aboutInfo" :contactsInfo="contactsInfo" :pagesInfo="pagesInfo" :blogInfo="blogInfo" />
</template>
<style></style>