<template>
  <MainLayout>
    Exemple using slot
  </MainLayout>
  <br>
  Props message:  {{ messages }}
</template>

<script setup>
import MainLayout from '../Layouts/MainLayout.vue';
defineProps(['messages'])
</script>

<style>

</style>