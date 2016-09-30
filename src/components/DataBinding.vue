<template>
    <div class="dataBinding">
        <p>绑定数据展示：{{ msg }}</p>
        <input v-model="msg">
    </div>
</template>

<script>
export default {
    data () {
        return {
            msg: 'Hello Vue.js !'
        }
    }
}
</script>