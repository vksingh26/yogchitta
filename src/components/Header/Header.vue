<template>
  <div class="header-container">
    <header class="header">
      <router-link to="/" class="logo"></router-link>
      <nav>
        <button class="menu-toggle" @click="toggleMenu">☰</button>
        <ul :class="{ 'nav-list': true, open: isMenuOpen }">
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/about">About</router-link></li>
          <li><router-link to="/contact">Contact</router-link></li>
        </ul>
      </nav>
    </header>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import './Header.css'

const isMenuOpen = ref(false)
function toggleMenu() {
  isMenuOpen.value = !isMenuOpen.value
}
</script>
