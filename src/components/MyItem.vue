<template>
  <div class="wrap item">
    <ul>
      <li 
        v-for="todo in todos"
        :key="todo.id"
      >
        <input type="checkbox" id="hobby">
        <label for="hobby">{{ todo.hobby }}</label>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'MyItem',
  props: ['todos']
}
</script>

<style scoped>
/* .item {
  
} */
  ul {
    padding: 0;
    margin: 0;
  }
  li {
    list-style: none;
    width: 100%;
    height: 30px;
  }
</style>