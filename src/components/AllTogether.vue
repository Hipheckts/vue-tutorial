<template>
    <div class="allTogether">
        <p>
            <label>请输入待办事项：</label>
            <input v-model="newTodo" @keyup.enter="addTodo" />
        </p>
        <p>待办事项列表：</p>
        <ul>
            <li v-for="todo in todos">
                {{ todo.text }}
                <i class="fa fa-trash"  @click="removeTodo($index)"></i>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    data () {
        return {
           newTodo: '',
           todos: [
                { text: '这是待办事项。' }
           ]
        }
    },
    methods: {
        addTodo () {
            let text = this.newTodo.trim()
            if (text) {
                this.todos.push({ text: text })
                this.newTodo = ''
            }
        },
        removeTodo (index) {
            this.todos.splice(index, 1)
        }
    }
}
</script>