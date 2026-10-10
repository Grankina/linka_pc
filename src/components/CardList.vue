<script setup>
import Card from './Card.vue'
</script>
<template>
  <div class="grid grid-cols-5 gap-5">
    <Card
      title="ROG G100 Edition 20(2025)"
      image-url="/computers/computer_1.webp"
      :price="73499"
      :isAdded="true"
      :isFavourite="true"
    />
    <Card title="ROG G170 Edition 20(2025)" image-url="/computers/computer_2.webp" :price="68900" />
    <Card />
    <Card />
    <Card />
  </div>
</template>
