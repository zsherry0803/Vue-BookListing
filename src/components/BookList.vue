<template>
  <div>
    <h1>{{title}}</h1>
  </div>
</template>

<script>
import BookItem from './BookItem';
import BookForm from './BookForm';
export default {
  name: 'BookList',
  data() {
    return {
      title: 'All Books'
    };
  },
  components: {
    BookItem,
    BookForm,
  },
  methods: {
    appendBook(bookTitle, bookAuthor) {
      this.books.push({ title: bookTitle, author: bookAuthor });
    },
  },
};
</script>

<style>
h1, h2 {
  font-weight: normal;
}
</style>