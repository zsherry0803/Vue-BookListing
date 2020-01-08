<template>
  <div>
    <ul>
      <li>{{book.title}}:{{book.author}}</li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "BookItem",
  props: ['book'],
};
</script>

<style>
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: block;
  margin: 0 10px;
}
</style>