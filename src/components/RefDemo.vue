<template>
    <div ref="container" class="container">{{ content }}</div>
    <input type="text" ref="username">
<button @click="getElementHandle">获取元素</button>
</template>

<script>

/**
 * 内容改变：{{模板语法}}
 * 属性改变：v-bind:指令
 * 事件：v-on:click
 * 
 * 如果沒有特別的要求，不要操作DOM
 */

export default {
    data() {
        return {
            content: "內容"
        }
    },
    methods:{
        getElementHandle(){
            // innerHTML:元素JS的属性
            //this.refs.container.innerHTML="1111"
            console.log(this.refs.username.value)
        }
    }
}
</script>