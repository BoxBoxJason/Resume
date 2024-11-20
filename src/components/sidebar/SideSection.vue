<template>
  <section class="sidebar-section">
    <h3 class="sidebar-section-title">{{ title }}</h3>
    <div class="sidebar-section-title-separator"></div>
    <slot />
    <div class="sidebar-section-separator"></div>
  </section>
</template>

<script>
export default {
  name: "SideBarSection",
  props: {
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.sidebar-section {
  margin-bottom: 20px;
}

.sidebar-section-title {
  font-size: 1.5em;
  margin: 0 0 5px;
}

.sidebar-section-title-separator {
  border-top: 1px solid #ddd;
  margin: 10px 0;
}

.sidebar-section-separator {
  border-top: 1px solid #ddd;
  margin: 10px 0;
}
</style>
