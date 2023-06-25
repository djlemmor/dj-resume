<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
import HelloWorld from './components/HelloWorld.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="You did it!" />

      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>
    </div>
  </header>
  <p class="text-2xl">
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Doloribus laborum illo officia et
    magnam reprehenderit culpa, cupiditate aspernatur. Recusandae rerum eveniet vel odit animi est
    quia voluptatibus consectetur quibusdam quidem! Lorem ipsum dolor sit, amet consectetur
    adipisicing elit. Dignissimos at quo consectetur tempore. Odio obcaecati nesciunt excepturi,
    quos delectus assumenda iusto exercitationem inventore, pariatur saepe voluptas, atque est at
    optio!
  </p>
  <RouterView />
</template>
