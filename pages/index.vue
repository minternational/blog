<template>
  <div>
    Hello World!
    {{ count }}
    <button @click="increment">Increment</button>
    <a href="/content">See Content</a>
  </div>
</template>

<script setup>
  definePageMeta({
    layout: "default",
  });

  const count = ref(0);
  const increment = () => count.value++
</script>