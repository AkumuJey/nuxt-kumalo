<template>
  <div class="bg-blue-50 h-screen flex flex-col">
    <header class="shadow-sm py-[1rem] px-[2rem]">
      <nav class="flex justify-between font-bold">
        <nuxt-link to="/">Nuxt Kumalo</nuxt-link>
        <ul class="flex gap-4">
          <li><nuxt-link to="/">Home</nuxt-link></li>
          <li><nuxt-link to="/about">About</nuxt-link></li>
          <li><nuxt-link to="/products">Products</nuxt-link></li>
        </ul>
      </nav>
    </header>
    <!-- Content -->
    <div class="grow py-[1rem] px-[0.5rem]">
      <slot />
    </div>
  </div>
</template>

<script setup lang="ts"></script>

<style lang="scss" scoped></style>
