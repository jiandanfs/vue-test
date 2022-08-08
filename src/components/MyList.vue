<template>
  <MyItem :todos="todos"/>
</template>

<script>
import MyItem from './MyItem.vue'

export default {
  name: 'MyList',
  props:['todos'],
  components: {
    MyItem
  },
  
}
</script>

<style scoped>

</style>