<template>
  <div class="my-name">
    <h1 class="green">Welcome, {{ name }}!</h1>
  </div>
</template>

<script setup>
defineProps({
  name: {
    type: String,
    required: true,
  },
})
</script>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

.my-name h1 {
  text-align: center;
}

@media (min-width: 1024px) {
  .my-name h1 {
    text-align: left;
  }
}
</style>
