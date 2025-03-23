<script setup lang="ts">
import { ref } from "vue";

defineProps<{ msg: string }>();

const count = ref(0);
</script>

<template>
  <div class="list history mt-[10px]">
    <div
      class="list-row history-item border-1 hover:bg-neutral-700 bg-neutral-800 border-neutral-800 rounded-[10px]"
      v-for="n in [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]"
    >
      <div>
        <div class="font-semibold text-[15px]">
          What is tailwind css? {{ n }}
        </div>
        <div class="font-light text-[12px]">03/23/2025</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.history-item {
  cursor: pointer;
}
</style>
