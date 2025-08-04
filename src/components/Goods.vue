<template>
  <div class="w-4/5 p-5 m-auto bg-white">
    <div class="text-3xl font-semibold">Все кроссовки</div>
    <div class="grid grid-cols-4">
      <div class="w-fit flex justify-between" v-for="(pop, index) in pops">
        <div class="mt-5 rounded-xl p-3 hover:-translate-y-2 hover:shadow-xl transition">
          <div class="relative cursor-pointer">
            <img class="absolute top-5 left-5" src="../public/img/like-1.png" alt="" />
            <img class="m-auto" :src="pop.img" alt="" />
            <div class="w-80">{{ pop.description }}</div>
            <div class="flex justify-between items-end">
              <div class="mt-4">
                <div class="text-slate-400">Цена:</div>
                <div class="font-bold text-xl">{{ pop.price }}</div>
              </div>
              <button @click="itemsBasketBtnState[index] = !itemsBasketBtnState[index]" class="active:translate-1 active:shadow-xl rounded-xl transition cursor-pointer">
                <img class="w-10" :src="itemsBasketBtnState[index] ? '../public/img/btn-2.png' : '../public/img/btn-1.png'" alt="" />
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  import { ref, onBeforeMount } from "vue";

  const pops = [
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-2.png",
      description: "Мужские Кроссовки Nike Air Max 270",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-3.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "8 499 руб.",
    },
    {
      img: "/img/boots-4.png",
      description: "Кроссовки Puma X Aka Boku Future Rider",
      price: "8 999 руб.",
    },
    {
      img: "/img/boots-5.png",
      description: "Мужские Кроссовки Under Armour Curry 8",
      price: "15 199 руб.",
    },
    {
      img: "/img/boots-6.png",
      description: "Мужские Кроссовки Nike Kyrie 7",
      price: "11 299 руб.",
    },
    {
      img: "/img/boots-7.png",
      description: "Мужские Кроссовки Jordan Air Jordan 11",
      price: "10 799 руб.",
    },
    {
      img: "/img/boots-8.png",
      description: "Мужские Кроссовки Nike LeBron XVIII",
      price: "16 499 руб.",
    },
    {
      img: "/img/boots-9.png",
      description: "Мужские Кроссовки Nike Lebron XVIII Low",
      price: "13 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "8 499 руб.",
    },
    {
      img: "/img/boots-4.png",
      description: "Кроссовки Puma X Aka Boku Future Rider",
      price: "8 999 руб.",
    },
    {
      img: "/img/boots-10.png",
      description: "Мужские Кроссовки Nike Kyrie Flytrap IV",
      price: "11 299 руб.",
    },
  ];

  const itemsBasketBtnState = ref([]);
</script>
