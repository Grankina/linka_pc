<script setup>
import Header from './Header.vue'
import CardItemList from './CardItemList.vue'
</script>
<template>
  <Header />
  <div class="p-10">
    <h2 class="text-3xl font-bold mb-8">Корзина</h2>
    <CardItemList />
    <div class="" flex flex-col gap-5 mb-6 my-6>
      <div class="flex">
        <span>Итого:</span>
        <p class="text-slate-400">2 товара</p>
        <div class="flex-1 border-b border-dashed">
          <b>200500 руб.</b>
        </div>
      </div>
      <buttom
        class="mt-4 transition bg-red-500 w-full rounded-xl py-4 text-white disabled:bg-slate-400 hover:bg-red-600 active:bg-red-700 cursor-pointer"
        >Оформить заказ</buttom
      >
    </div>
  </div>
</template>
