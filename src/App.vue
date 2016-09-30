<template>
    <div id="app">
        <!-- hello world -->
        <div class="demo">
            <div class="title">练习：1 —— Hello</div>
            <hello></hello>
        </div>
        <!-- 双向数据绑定 -->
        <div class="demo">
            <div class="title">练习：2 —— 双向数据绑定</div>
            <data-binding></data-binding>
        </div>
        <!-- 渲染列表 -->
        <div class="demo">
            <div class="title">练习：3 —— 渲染列表</div>
            <render-list></render-list>
        </div>
        <!-- 处理用户输入 -->
        <div class="demo">
            <div class="title">练习：4 —— 处理用户输入</div>
            <handle-user-input></handle-user-input>
        </div>
        <!-- 综合 -->
        <div class="demo">
            <div class="title">练习：5 —— 综合</div>
            <all-together></all-together>
        </div>
    </div>
</template>

<script>
import Hello from './components/Hello'
import DataBinding from './components/DataBinding'
import RenderList from './components/RenderList'
import HandleUserInput from './components/HandleUserInput'
import AllTogether from './components/AllTogether'

export default {
  components: {
    Hello,
    DataBinding,
    RenderList,
    HandleUserInput,
    AllTogether
  }
}
</script>
<style>
    body {
        padding: 20px;
    }
</style>
<style scoped>
    .demo {
        background: #f4f4f4;
        border-radius: 4px;
        border: 1px solid #eee;
        padding: 20px;
        .title {
            padding-bottom: 10px;
            font-weight: 600;
            font-size: 1.2em;
            color: #2c3e50;
            border-bottom: 1px solid #ccc;
        }
        &+.demo {
            margin-top: 20px;
        }
    }
</style>