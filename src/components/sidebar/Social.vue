<template>
  <div class="social">
    <img :src="illustration" :alt="name" class="social-icon" />
    <a :href="url" class="social-name">{{ name }}</a>
  </div>
</template>

<script>
export default {
  name: "Social",
  props: {
    illustration: {
      type: String,
      required: true,
    },
    name: {
      type: String,
      required: true,
    },
    url: {
      type: String,
      required: false,
      default: null,
    }
  }
};
</script>

<style scoped>
.social {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.social-icon {
  width: 30px;
  height: 30px;
  margin-right: 10px;
}

.social-name {
  font-size: 1.2em;
  color: #333;
  text-decoration: none;
}

.social-name:hover {
  text-decoration: underline;
}
</style>