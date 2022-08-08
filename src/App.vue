<template>
  <div class="app">
    <MyHeader />
    <MyList :todos="todos"/>
    <MyFooter />
  </div>
</template>

<script>
import MyHeader from "./components/MyHeader.vue";
import MyList from "./components/MyList.vue";
import MyFooter from "./components/MyFooter.vue";
import {nanoid} from "nanoid"
export default {
  name: "App",
  components: {
    MyHeader,
    MyList,
    MyFooter
  },
  data() {
    return {
      todos: [
        {id: nanoid(),hobby: "吃饭",done: true},
        {id: nanoid(),hobby: "睡觉",done: true},
      ]
    }
  }
};
</script>

<style>
  .app {
    padding: 10px;
    width: 400px;
    margin: 0 auto;
    
  }
  .app, .wrap {
    border-radius: 5px;
    border: 1px solid gray;
    margin-top: 5px;
  }

  .wrap {
    width: 100%;
  }
</style>
