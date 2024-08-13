<template>
  <div class="border-b border-t border-slate-300 py-2 w-1/2 cursor-pointer">
    <div class="flex items-center gap-x-16 relative">
      <div class="flex items-center space-x-2 mr-12">
        <img :src="item.img" alt="" />
        <span v-if="item.title" class="text-2xl pt-2">{{ item.title }}</span>
      </div>
      <img src="/bottoarrow.svg" alt="" class="absolute right-0 transition hover:rotate-180" />
    </div>
    <p>
      {{ item.text }}
    </p>
  </div>
</template>

<script setup>
defineProps({
  item: {
    type: Object
  }
})
</script>

<style lang="scss" scoped></style>
