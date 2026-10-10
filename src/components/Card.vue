<script setup>
defineProps({
  title: String,
  imageUrl: String,
  price: Number,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClickAdd: Function,
  onClickFavorite: Function,
})
</script>
<template>
  <div>
    <div
      class="relative border bg-white border-slate-300 rounded-xl p-8 cursor-pointer transition hover:-translate-y-2 hover:shadow-xl"
    >
      <img
        :src="!isFavourite ? 'like-1.svg' : 'like-2.svg'"
        alt="Like"
        class="absolute top-8 left-8"
        @click="onClickFavorite"
      />
      <img :src="imageUrl" alt="Computer" class="w-40" />
      <p>{{ title }}</p>
      <div class="flex justify-between">
        <div class="flex flex-col">
          <span class="text-slate-400">Цена:</span>
          <span>{{ price }} руб.</span>
        </div>
        <img @click="onClickAdd" :src="!isAdded ? '/plus.svg' : '/checked.svg'" alt="Plus" />
      </div>
    </div>
  </div>
</template>
