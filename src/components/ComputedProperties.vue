<template>
  <p>Has published books:</p>
  <div>
    <span>{{ publishedBooksMessage }}</span>
  </div>
  <button @click="deleteBooks">Delete Books</button>
</template>

<script>
export default {
  data() {
    return {
      author: {
        name: "John Doe",
        books: ["Vue 2 - Advanced Guide", "Vue 3 - Basic Guide", "Vue 4 - The Mystery"],
      },
    };
  },
  computed: {
    publishedBooksMessage() {
      return this.author.books.length > 0 ? "Yes" : "No";
    },
  },
  methods: {
    deleteBooks() {
      this.author.books = [];
    },
  },
};
</script>

<style></style>
