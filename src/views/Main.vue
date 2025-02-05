<template>
  <div class="w-screen h-screen flex gap-0 text-sm">
    <Navbar />
    <div class="flex-auto bg-slate-100 py-2 px-1">
      <div
        class="rounded-lg py-2 px-4 flex justify-between bg-white border-b border-gray-200"
      >
        <div class="flex items-center gap-2.5">
          <img
            src="https://lalals.s3.amazonaws.com/images/Ava%20Max%20AI.jpg"
            alt=""
            class="h-8 w-8 rounded-full object-contain"
          />
          <span class="text-base font-medium">Hoàng Mạnh (Bot Bán Hàng)</span>
          <PenSvg />
        </div>
        <button
          class="h-8 w-8 bg-gray-200 rounded-full p-1.5 flex justify-center items-center"
        >
          <TableCellsIcon class="text-black h-5 w-5" />
        </button>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import Navbar from "@/components/layout/nav-bar/Navbar.vue"
import { TableCellsIcon } from "@heroicons/vue/24/solid"
import PenSvg from "@/assets/icons/pen.vue"
</script>
