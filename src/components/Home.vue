<template>
  <div>
    <ul v-if="toDoList && toDoList.length">
      <li v-for="(toDoItem, index) in toDoList" v-bind:key="index">
        <p>
          <strong>{{toDoItem.id + ' - '+ toDoItem.title + ' - '+ toDoItem.completed }}</strong>
        </p>
      </li>
    </ul>

    <ul v-if="errors && errors.length">
      <li v-for="(error, index) in errors" v-bind:key="index">{{ error.message }}</li>
    </ul>
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