<script setup>
import Card from './Card.vue'

defineProps({
  items: Array,
})

</script>

<template>
  <div class="grid grid-cols-4 gap-5" v-auto-animate>
    <Card
      v-for="item in items"
      :key="item.id"
      :id="item.id"
      :title="item.title"
      :image="item.image"
      :author="item.author"
    />
  </div>
</template>
