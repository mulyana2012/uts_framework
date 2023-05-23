<script setup>
import { RouterLink, RouterView } from 'vue-router';
</script>

<template>
  <header>
    <ul class="nav justify-content-center" style="background-color: rgb(9, 62, 132)">
      <li class="nav-item">
        <a class="nav-link text-light" href="/">CLUB</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" text-light href="/lives">LAGA</a>
      </li>
      <li class="nav-item">
        <a class="nav-link text-light" href="#">ABOUT</a>
      </li>
    </ul>
  </header>

  <RouterView />
</template>
