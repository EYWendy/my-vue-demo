<template>
    <h3>表单输入与绑定</h3>
    <form>
        <input type="text" v-model.lazy="message">
        <p>{{ message }}</p>

        <input type="checkbox" id="checkbox" v-model="checked">
        <label for="checkbox">{{checked}}</label>

    </form>

</template>

<script>
export default {
    data() {
        return {
            message: "",
            checked:false
        }
    }
}
</script>