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

const toDoList = [toDoItem1, toDoItem2, toDoItem3];

</script>

<template>

    <h1>To Do List</h1>

    <table class="table">
        <thead>
            <tr>
                <th scope="col">Id</th>
                <th scope="col">Name</th>
                <th scope="col">Is Completed</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th scope="row">{{ toDoList[0].id }}</th>
                <td>{{ toDoList[0].name }}</td>
                <td>{{ toDoList[0].isCompleted }}</td>
            </tr>
            <tr>
                <th scope="row">{{ toDoList[1].id }}</th>
                <td>{{ toDoList[1].name }}</td>
                <td>{{ toDoList[1].isCompleted }}</td>
            </tr>
            <tr>
                <th scope="row">{{ toDoList[2].id }}</th>
                <td>{{ toDoList[2].name }}</td>
                <td>{{ toDoList[2].isCompleted }}</td>
            </tr>
        </tbody>
    </table>
</template>
