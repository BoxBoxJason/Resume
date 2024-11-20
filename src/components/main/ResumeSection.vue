<template>
  <section class="resume-section">
    <h3 class="resume-section-title">{{ title }}</h3>
    <div class="resume-section-title-separator"></div>
    <slot />
  </section>
</template>

<script>
export default {
  name: "ResumeSection",
  props: {
    title: {
      type: String,
      required: true,
    },
  },
};
</script>

<style scoped>
.resume-section {
  margin-bottom: 20px;
}

.resume-section-title {
  font-size: 1.5em;
  margin: 0 0 5px;
}

.resume-section-title-separator {
  border-top: 1px solid #ddd;
  margin: 10px 0;
}
</style>
