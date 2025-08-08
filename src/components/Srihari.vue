<script setup>
defineProps({
  msg: {
    type: String,
    required: false,
  },
})
</script>

<template>
  <div class="testing">
    <h1 class="green">{{ msg }}</h1>
    <h3>
      My custom testing component.
    </h3>
  </div>
</template>

<style scoped>
h1 {
  font-weight: 500;
  font-size: 2.6rem;
  position: relative;
  top: -10px;
}

h3 {
  font-size: 1.2rem;
}

.testing h1,
.testing h3 {
  text-align: center;
}

@media (min-width: 1024px) {
  .testing h1,
  .testing h3 {
    text-align: left;
  }
}
</style>
