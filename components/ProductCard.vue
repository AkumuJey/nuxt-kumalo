<template>
  <div class="card tex-center bg-slate-50 rounded-md p-3">
    <img :src="product.image" :alt="product.title" class="thumb" />
    <p class="font-bold text-gray-500 m-4 truncate">{{ product.title }}</p>
    <NuxtLink :to="`/products/${product.id}`">
      <p class="py-2 px-3 my-4 bg-teal-500 rounded-sm">View details</p>
    </NuxtLink>
  </div>
</template>

<script setup>
const { product } = defineProps(["product"]);
</script>

<style scoped>
.thumb {
  max-height: 120px;
  max-width: 70%;
  margin: 0 auto;
}
</style>
