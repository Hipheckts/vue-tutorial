<template>
    <div class="handleUserInput">
        <p>展示处理：{{ msg }}</p>
        <button @click="reverseMsg">取反</button>
    </div>
</template>

<script>
export default {
    data () {
        return {
            msg: 'Hello Vue.js!'
        }
    },
    methods: {
      reverseMsg () {
        this.msg = this.msg.split('').reverse().join('')
      }
    }
}
</script>