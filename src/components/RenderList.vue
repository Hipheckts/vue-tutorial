<template>
    <div class="renderList">
        <ul>
            <li v-for="item in jsLibs">
                {{ item.name }}
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    data () {
        return {
            jsLibs: [
                { name: 'React.js' },
                { name: 'Vue.js' },
                { name: 'Angular.js' }
            ]
        }
    }
}
</script>