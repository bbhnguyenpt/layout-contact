<template>
  <div class="rounded-lg py-2 px-3 bg-white flex flex-col gap-2">
    <div class="flex items-center justify-between">
      <span class="text-2xl font-semibold">Danh bạ</span>
      <div class="flex items-center gap-3">
        <button
          class="py-2 px-3 rounded-lg bg-blue-700 text-white font-medium transition-all hover:bg-blue-800"
        >
          Tạo mới
        </button>
        <button>
          <EllipsisVerticalIcon class="h-6 w-6 text-gray-600" />
        </button>
      </div>
    </div>
    <div class="flex justify-between">
      <div class="flex gap-2.5">
        <button
          class="h-[30px] w-[30px] flex justify-center items-center rounded-full bg-gray-200"
        >
          <MagnifyingGlassIcon class="text-black h-3.5 w-3.5" />
        </button>
        <button
          class="h-[30px] w-[30px] flex justify-center items-center rounded-full bg-gray-200"
        >
          <ArrowsUpDownIcon class="text-black h-3.5 w-3.5" />
        </button>
        <button
          class="h-8 bg-gray-200 rounded-3xl p-2 flex items-center gap-1 text-black"
        >
          <CalendarDaysIcon class="h-3.5 w-3.5" />
          <span class="text-xs font-medium">Thời gian</span>
          <ChevronDownIcon class="h-4 w-4" />
        </button>
      </div>
      <button
        class="h-9 w-9 flex justify-center items-center rounded-full bg-gray-200"
      >
        <MagnifyingGlassIcon
          class="text-black h-5 w-5 stroke-black stroke-[0.5]"
        />
      </button>
    </div>
    <div class="flex justify-between text-black">
      <div class="flex flex-col gap-0">
        <div class="flex gap-2.5 items-center">
          <span class="text-base font-semibold">Qualified</span>
          <ChevronDownIcon class="h-5 w-5" />
        </div>
        <span class="text-xs font-medium">Lead</span>
      </div>
      <span class="text-base font-semibold">31</span>
    </div>
  </div>
</template>

<script setup lang="ts">
import {
  EllipsisVerticalIcon,
  MagnifyingGlassIcon,
  ArrowsUpDownIcon,
  CalendarDaysIcon,
  ChevronDownIcon,
} from "@heroicons/vue/24/solid"
</script>
