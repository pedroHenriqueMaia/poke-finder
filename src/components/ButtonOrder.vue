<script setup>
import IconOrder from '@/assets/icons/order.svg?component'
const emit = defineEmits(['order-by'])
</script>

<template>
  <div class="mb-8">
    <button class="ml-3 inline-flex gap-2 items-center h-10 px-3 rounded active:text-black/60 border border-black/5 border-b-black/40 bg-white/70 hover:bg-neutral-900/5 active:bg-neutral-700/5 active:border-black/5 outline outline-2 outline-offset-1 outline-transparent focus-visible:outline-black transition-all"  @click="emit('order-by', 'name')">
      Nome<IconOrder class="w-4 h-4" />
    </button>
    <button class="ml-3 inline-flex gap-2 items-center h-10 px-3 rounded active:text-black/60 border border-black/5 border-b-black/40 bg-white/70 hover:bg-neutral-900/5 active:bg-neutral-700/5 active:border-black/5 outline outline-2 outline-offset-1 outline-transparent focus-visible:outline-black transition-all"  @click="emit('order-by', 'id')">
      ID<IconOrder class="w-4 h-4" />
    </button>
  </div>
</template>