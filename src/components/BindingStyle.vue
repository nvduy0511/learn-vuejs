<template>
  <div :style="{ color: activeColor, fontSize: fontSize + 'px' }">Binding Style</div>
  <button @click="toggleStyle">Change Style</button>
</template>

<script>
export default {
  data() {
    return {
      activeColor: "red",
      fontSize: 50,
    };
  },
  methods: {
    toggleStyle() {
      this.activeColor = "green";
      this.fontSize = 20;
    },
  },
};
</script>

<style></style>
