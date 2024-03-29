<script setup>
import MainLayout from '../components/MainLayout.vue';
import Homecode from '../components/Homecode.vue';


// Page Title of Views
const pageTitle = 'Home'
</script>

<template>
  <MainLayout :pageTitle="pageTitle">


    <Homecode />


  </MainLayout>
</template>
