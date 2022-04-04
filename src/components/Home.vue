<template>
  <div>
    <h1>To Do List</h1>
    <table class="table">
      <thead>
        <tr>
          <th scope="col">
            <strong>Id</strong>
          </th>
          <th scope="col">
            <strong>Name</strong>
          </th>
          <th scope="col">
            <strong>Is Completed</strong>
          </th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(toDoItem, index) in toDoList" v-bind:key="index">
          <th scope="row">{{ toDoItem.id }}</th>
          <td>{{ toDoItem.title }}</td>
          <td>{{ toDoItem.completed }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
import axios from 'axios';

export default {
  data() {
    return {
      toDoList: [],
      errors: []
    }
  },

  // Fetches toDoList when the component is created.
  created() {
    axios.get(`https://jsonplaceholder.typicode.com/todos`)
      .then(response => {
        // JSON responses are automatically parsed.
        this.toDoList = response.data
      })
      .catch(e => {
        this.errors.push(e)
      })
  }
}
</script>