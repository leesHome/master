<template>
    <div class="headers">
        <span><a :href="{}">注册</a>&nbsp;|&nbsp;<a :href="{}">登录</a></span>
        <a :href="{}">APP下载</a>
    </div>
</template>

<script>
    export default {
        name: "header"
    }
</script>

<style scoped>
    .headers{
        height: 4rem;
        width: 100%;
        color: red;
        font-size: 1.8rem;
        line-height: 4rem;
        /* background: url(http://m.jr.jd.com/spe/qyy/main/images/jr-logo.png) no-repeat center; */
        background-size: auto 50%;
        z-index: 100;
    }
    .headers span a{
        color: red;
    }
    .headers span{
        height: 100%;
        display: inline-block;
        margin-left: 2rem;
    }
    .headers>a{
        float: right;
        height: 2rem;
        line-height: 2rem;
        margin-top: 1rem;
        margin-right: 1rem;
        color: white;
        background-color: red;
        padding: 0.2rem 0.4rem;
        border-radius: 0.3rem;
    }
</style>