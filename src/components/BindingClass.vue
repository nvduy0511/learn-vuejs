<template>
  <h2 :class="{ 'is-active': isActive }">Is Active</h2>
  <button @click="toggleIsActive">Toggle Is Active</button>
</template>

<script>
export default {
  data() {
    return {
      isActive: true,
    };
  },
  methods: {
    toggleIsActive() {
      this.isActive = !this.isActive;
    },
  },
};
</script>

<style scoped>
h2 {
  color: red;
}

.is-active {
  color: green;
}
</style>
