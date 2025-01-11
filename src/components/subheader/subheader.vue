<template>
  <section class="subheader">
    <div class="subheader-container">
      <div class="subheader-contents">
        <div class="subheader-social">
          <router-link to="" class="instagram" @click="openInstagramLink"></router-link>
          <router-link to="" class="whatsapp" @click="openWhatsappLink"></router-link>
          <router-link to="" class="youtube" @click="openYoutubeLink"></router-link>
        </div>
        <div class="subheader-info">
          <router-link to="/about" class="border-bottom" :active-class="'active-link'"
            >about yogchitta</router-link
          >
          <router-link to="/contact" class="border-bottom" :active-class="'active-link'"
            >contact</router-link
          >
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import './subheader.css'

function openInstagramLink(event) {
  event.preventDefault() // Prevent Vue Router from handling the click
  window.open('https://www.instagram.com/yogchitta/', '_blank') // Open Instagram in a new tab
}

function openWhatsappLink(event) {
  event.preventDefault() // Prevent Vue Router from handling the click
  window.open('https://api.whatsapp.com/send?phone=9406509760', '_blank') // Open Whatsapp in a new tab;
}

function openYoutubeLink(event) {
  event.preventDefault() // Prevent Vue Router from handling the click
  window.open('https://www.youtube.com/@yogchitta', '_blank') // Open Whatsapp in a new tab;
}
</script>
