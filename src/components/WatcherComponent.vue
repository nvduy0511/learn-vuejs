<template>
  <div class="my-component">
    <input v-model="message.title" />
    <div>{{ message.title }}</div>
    <div><button @click="changeMessage">Click me</button></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      message: {
        title: "This is message",
        length: 10,
      },
    };
  },
  watch: {
    message: {
      handler(newValue, oldValue) {
        console.log({ oldValue });
        console.log({ newValue });
      },
      // immediate: true
      // deep:true
    },
  },
  methods: {
    changeMessage() {
      this.message.title = "Demo Watcher In VueJs";
    },
  },
};
</script>

<style scoped>
.my-component {
  color: red;
}
</style>
