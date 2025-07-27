<template>
  <div class="flex justify-center items-center border-2 mt-5">
    <div class="flex flex-col items-center">
      <div class="text-2xl">Товар:</div>
      <div class="text-2xl">{{ title }}</div>
      <div class="text-2xl mt-5">Цена: {{ price }}</div>
      <slot></slot>
    </div>
  </div>
</template>

<script setup>
  defineProps({
    title: String,
    price: Number,
  });
</script>
