<template>
  <MyHello title="Кросовки Puma" :price="9500">
    <button class="btn">lol</button>
  </MyHello>
  <MyHello title="Кросовки lol" :price="8400">
    <div>lol</div>
  </MyHello>
  <MyHello title="Кросовки kek" :price="7300"></MyHello>
  <MyHello title="Кросовки apchi" :price="6200"></MyHello>
</template>

<script setup>
  import MyHello from "./components/MyHello.vue";
</script>
