<template>
  <div class="w-4/5 p-5 m-auto bg-white">
    <div class="text-3xl font-semibold">Все кроссовки</div>
    <div class="grid grid-cols-4">
      <div class="w-fit flex justify-between" v-for="pop in pops">
        <div class="mt-5 rounded-xl p-3 hover:-translate-y-2 hover:shadow-xl transition">
          <div class="relative cursor-pointer">
            <img class="absolute top-5 left-5 w-10" src="../public/img/like-1.png" alt="" />
            <img class="m-auto" src="../public/img/boots-1.png" alt="" />
            <div>{{ pop.description }}</div>
            <div class="flex justify-between items-end">
              <div class="mt-4">
                <div class="text-slate-400">Цена:</div>
                <div class="font-bold text-xl">{{ pop.price }}</div>
              </div>
              <button class="btn bg-white rounded-xl border-2 border-gray-300 text-xl text-gray-500">+</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
  const pops = [
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
    {
      img: "/img/boots-1.png",
      description: "Мужские Кроссовки Nike Blazer Mid Suede",
      price: "12 999 руб.",
    },
  ];
</script>
