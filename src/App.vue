<script setup>
import { RouterLink, RouterView } from 'vue-router';
</script>

<template>
  <header>
    <nav class="nav" style="background-color: #1b9c85">
      <a class="nav-link text-white" href="/">CLUB</a>
      <a class="nav-link text-white" href="/lives">LAGA</a>
      <a class="nav-link text-white" href="/">ABOUT</a>
    </nav>
  </header>

  <RouterView />
</template>
