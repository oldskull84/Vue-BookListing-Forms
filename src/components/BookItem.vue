<template>
  <li>
    <div>
    {{ book.title }} : {{ book.author }}
    </div>
    <span v-if="book.finishedReading">Read</span>
    <span v-else>Not Read</span>
  </li>
</template>

<script>
export default {
  name: "BookItem",
  props: ["book"],
};
</script>

<style>
li {
  display: block;
  margin: 0 10px;
}
</style>