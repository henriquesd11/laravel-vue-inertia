<template>
  <div>
    <Link href="/"> Index </Link>
    <Link href="show"> Show </Link>
    <div>Page with time {{ timer }}</div>
  </div>
  <slot/>
</template>

<script setup>
import {Link} from '@inertiajs/inertia-vue3'
import { ref } from 'vue';

const timer = ref(0);
setInterval(() => {
  timer.value++;
}, 1000);
</script>

<style>

</style>