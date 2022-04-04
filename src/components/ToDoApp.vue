<script setup>

const toDoItem1 = {
    id: 1,
    name: "to Do Item 1",
    isCompleted: true
};
const toDoItem2 = {
    id: 2,
    name: "to Do Item 2",
    isCompleted: false
};
const toDoItem3 = {
    id: 3,
    name: "to Do Item 3",
    isCompleted: true
};
const toDoItem4 = {
    id: 4,
    name: "to Do Item 4",
    isCompleted: false
};
const toDoList = [toDoItem1, toDoItem2, toDoItem3, toDoItem4];

</script>

<template>
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
                <td>{{ toDoItem.name }}</td>
                <td>{{ toDoItem.isCompleted }}</td>
            </tr>
        </tbody>
    </table>
</template>
