<template>
  <div class="todo">
    <input v-model="input" type="text" />
    <button v-on:click="todos.push(input)">Add</button>

    <ul>
      <li v-for="todo in todos" :key="todo">
        {{ todo }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "ToDo",
  data() {
    return {
      todos: [],
      input: "",
    };
  },
};
</script>

<style scoped>
.todo {
  width: 60%;
  margin: 20px auto;
}
</style>
