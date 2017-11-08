<template>
<div class="iconfont icon-top" @click="goTop">&#xe611;</div>
</template>
<script>
    export default {
        replace: true,
        methods: {
            goTop() {
                // $(window).scrollTop(0);
                // this.show = false;
                this.$router.go(-1);
            }
        }
    };
</script>
<style>
    .icon-top {
        position: fixed;
        right: 10px;
        bottom: 80px;
        font-size: 50px;
        z-index: 9999;
        color: #42b983;
    }
</style>