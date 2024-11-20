<template>
  <aside class="sidebar">
    <img class="sidebar-avatar" :src="avatar" alt="avatar" />
    <slot />
  </aside>
</template>

<script>
export default {
  name: "SideBar",
  props: {
    avatar: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.sidebar {
  margin: 0 auto;
  max-width: 200px;
  padding: 20px;
}
</style>
