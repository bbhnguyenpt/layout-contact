<template>
  <nav
    class="p-2 flex flex-col gap-3 bg-slate-100 w-[330px] h-full overflow-y-auto"
  >
    <NavHeading />
    <div class="bg-white rounded-xl py-3 flex flex-col gap-5">
      <ListUser
        v-for="(list, index) in NAV_DUMB_DATA"
        :key="index"
        :label="list.label"
        :list_user="list.list_user"
      />
    </div>
  </nav>
</template>

<script setup lang="ts">
import ListUser from "./ListUser.vue"
import NavHeading from "./NavHeading.vue"

const NAV_DUMB_DATA = [
  {
    label: "HÔM NAY 18/07/2024",
    list_user: new Array(5).fill(0),
  },
  {
    label: "HÔM QUA 17/07/2024",
    list_user: new Array(7).fill(0),
  },
  {
    label: "HÔM KIA 16/07/2024",
    list_user: new Array(7).fill(0),
  },
]
</script>
