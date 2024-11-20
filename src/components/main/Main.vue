<template>
  <header class="main">
    <h1 class="main-title">{{ surname }} {{ name }}</h1>
    <h2 class="main-subtitle">{{ title }}</h2>
  </header>
  <slot />
</template>

<script>
export default {
  name: "Main",
  props: {
    name: {
      type: String,
      required: true,
    },
    surname: {
      type: String,
      required: true,
    },
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.main {
  margin: 0 auto;
  max-width: 800px;
  padding: 20px;
}

.main-title {
  font-size: 2em;
  margin: 0 0 5px;
}

.main-subtitle {
  font-size: 1.5em;
  margin: 0 0 20px;
}
</style>
