<template>
  <subheader />
  <Header />
  <RouterView />
</template>

<script setup>
import { RouterView } from 'vue-router'
import subheader from '@/components/subheader/subheader.vue'
import Header from '@/components/Header/Header.vue'
</script>
<style scoped></style>
