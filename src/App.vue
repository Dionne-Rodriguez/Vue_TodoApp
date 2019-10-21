<template>
  <div id="app">
    <Todos v-bind:todos="todos"/>
  </div>

</template>

<script>

import Todos from './components/Todo';


export default {
  name: 'app',
  components: {
      Todos 
  },
  data(){
    return{
      todos: [
        {
          id:1,
          title: 'Todo one',
          completed: false
        },
         {
          id:2,
          title: 'Todo two',
          completed: false
        },
         {
          id:3,
          title: 'Todo three',
          completed: true
        }
      ]
    }
  }

}
</script>

<style>
*{
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}
body{
  line-height: 1.4;
  font-family: Arial, Helvetica, sans-serif
}
</style>
