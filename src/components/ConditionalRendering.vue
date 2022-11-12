<template>
  <input v-model="type" />
  <div v-if="type === 'A'">A</div>
  <div v-else-if="type === 'B'">B</div>
  <div v-else-if="type === 'C'">C</div>
  <div v-else>Not A/B/C</div>
  <h1 v-show="type === 'A'">A v-show</h1>
</template>

<script>
export default {
  data() {
    return {
      type: "B",
    };
  },
};
</script>

<style></style>
