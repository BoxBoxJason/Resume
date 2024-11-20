<template>
  <div class="resume" :id="resumeId">
    <slot />
  </div>
</template>

<script>
export default {
  name: "Resume",
  props: {
    resumeId: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.resume {
  margin: 0 auto;
  max-width: 800px;
  padding: 20px;
}
</style>
