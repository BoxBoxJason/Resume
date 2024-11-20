<template>
  <article class="section-item">
    <a v-if="link" :href="link">
      <h4 class="section-item-title">{{ title }}</h4>
    </a>
    <h4 v-else class="section-item-title">{{ title }}</h4>
    <div class="section-item-header">
      <time class="section-item-date" :datetime="machineDatetime">{{ date }}</time>
      <span v-if="location" class="section-item-location">- {{ location }}</span>
    </div>
    <div class="section-item-content">
      <slot />
    </div>
  </article>
</template>

<script>
export default {
  name: "SectionItem",
  props: {
    title: {
      type: String,
      required: true,
    },
    date: {
      type: String,
      required: true,
    },
    machineDatetime: {
      type: String,
      required: false,
      default: null,
    },
    location: {
      type: String,
      required: false,
      default: null,
    },
    link: {
      type: String,
      required: false,
      default: null,
    },
  },
};
</script>

<style scoped>
.section-item {
  margin-bottom: 20px;
  padding: 10px;
  border: 1px solid #ddd;
  border-radius: 5px;
}

.section-item-title {
  font-size: 1.5em;
  margin: 0 0 5px;
}

.section-item-header {
  font-size: 0.9em;
  color: #555;
  margin-bottom: 10px;
}

.section-item-location {
  margin-left: 5px;
}

.section-item-content {
  font-size: 1em;
  color: #333;
}
</style>
