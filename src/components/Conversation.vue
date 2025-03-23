<script setup lang="ts">
import { ref } from "vue";

defineProps<{}>();
</script>

<template>
  <div
    class="conversation border-b-1 border-neutral-700 p-3"
    v-for="_ in [1, 2, 3, 4, 5, 6]"
  >
    <div class="conversation-me">What is TailwindCSS?</div>
    <div class="conversation-reply">
      Tailwind CSS is a powerful utility-first framework that allows developers
      to create responsive and customizable designs efficiently. Unlike
      traditional CSS frameworks that provide pre-designed components, Tailwind
      focuses on low-level utility classes, enabling developers to build unique
      UI designs without writing custom CSS. This approach not only speeds up
      development but also ensures a consistent design system across
      applications. Additionally, Tailwind’s configuration file allows for
      extensive customization, making it adaptable to different project
      requirements. One of the standout features of Tailwind CSS is its
      responsive design utilities, which simplify creating layouts for different
      screen sizes. With classes like sm:grid-cols-2 or lg:w-1/2, developers can
      adjust element styles based on the viewport without needing media queries.
      This makes Tailwind an excellent choice for modern web development,
      especially for teams that prioritize maintainability and scalability. As a
      result, many developers have adopted Tailwind for projects ranging from
      personal websites to enterprise applications.
    </div>
  </div>
</template>

<style scoped>
.conversation-me {
  padding: 10px 30px;
  margin-bottom: 10px;
  border-radius: 30px;
  margin-top: 10px;
  text-align: right;
  background-color: oklch(0.269 0 0);
}
.conversation-reply {
  padding: 10px;
  margin-bottom: 10px;
}
</style>
