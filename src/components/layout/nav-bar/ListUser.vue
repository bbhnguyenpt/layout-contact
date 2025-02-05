<template>
  <div class="px-2 flex flex-col gap-2">
    <div
      class="py-1 px-2 rounded bg-slate-100 flex justify-between items-center text-xs font-semibold text-slate-700 sticky top-0"
    >
      <span>{{ label }}</span>
      <span>{{ list_user.length }}</span>
    </div>
    <div class="flex flex-col gap-2 overflow-hidden">
      <ListUserItem v-for="(item, index) in list_user" :key="index" />
    </div>
  </div>
</template>

<script setup lang="ts">
import ListUserItem from "./ListUserItem.vue"

defineProps<{
  label: string
  list_user: any[]
}>()
</script>
