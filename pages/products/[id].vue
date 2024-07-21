<template>
  <div class="h-full w-full">
    <h3>{{ product.title }}</h3>
    <p>{{ product.price }}</p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;

const uri = "https://fakestoreapi.com/products/" + id;

const { data: product } = await useFetch(uri, {
  key: id,
});
</script>

<style lang="scss" scoped></style>
