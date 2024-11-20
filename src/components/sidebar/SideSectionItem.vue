<template>
    <article class="side-section-item">
      <h4 class="side-section-item-title">{{ title }}</h4>
      <div class="section-item-content">
        <slot />
      </div>
    </article>
  </template>

  <script>
  export default {
    name: "SideSectionItem",
    props: {
      title: {
        type: String,
        required: true,
      },
    },
  };
  </script>

  <style scoped>
  .side-section-item {
    margin-bottom: 20px;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
  }

  .side-section-item-title {
    font-size: 1.5em;
    margin: 0 0 5px;
  }

  .side-section-item-header {
    font-size: 0.9em;
    color: #555;
    margin-bottom: 10px;
  }

  .side-section-item-content {
    font-size: 1em;
    color: #333;
  }
  </style>
