<script setup lang="ts">
import { ref } from "vue";

defineProps<{}>();
</script>

<template>
  <div class="flex w-full h-full">
    <textarea
      class="textarea textarea-md bg-neutral-900 w-full h-full border-none focus:outline-0"
      placeholder="Enter message here."
    ></textarea>
    <button
      id="send-input"
      class="btn btn-soft btn-sm absolute right-[20px] bottom-[25px]"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        fill="none"
        viewBox="0 0 24 24"
        stroke-width="1.5"
        stroke="currentColor"
        class="size-6"
      >
        <path
          stroke-linecap="round"
          stroke-linejoin="round"
          d="M6 12 3.269 3.125A59.769 59.769 0 0 1 21.485 12 59.768 59.768 0 0 1 3.27 20.875L5.999 12Zm0 0h7.5"
        />
      </svg>
      Send
    </button>
  </div>
</template>

<style scoped>
.textarea {
  resize: none;
}
</style>
