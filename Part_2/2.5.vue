<template>
    <div id="app">
        <p v-if="show">这是一段文本</p>
        <button v-on:click="handClose">点击隐藏</button>
    </div>
</template>

<script>
    export default {
        name: "2.5"
    }

    var app = new Vue ({
        el: '#app',
        data: {
            show: true
        },
        methods: {
            handleClose: function () {
                this.show = false;
            }
        }
    })
</script>

<style scoped>

</style>