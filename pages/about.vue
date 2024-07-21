<template>
  <div>
    <h3>About</h3>
    <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Dicta ab cum est
      cumque optio ex rerum non soluta, inventore, recusandae eos laboriosam
      fugiat officiis exercitationem!
    </p>
  </div>
</template>

<script setup lang="ts">
interface Rating {
  rate: number;
  count: number;
}

interface Product {
  title: string;
  price: number;
  description: string;
  image: string;
  rating: Rating;
  category: string;
}
useHead({
  title: "Nuxt Kumalo | About",
});
</script>

<style scoped>
h3 {
  font-size: 20px;
}
</style>
