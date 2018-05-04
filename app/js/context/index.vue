<template>
    <div>
        <Lunbo></Lunbo>
    </div>
</template>

<script>
    import Lunbo from '../lunbo/index'
    export default {
        name: "index",
        components: {
            Lunbo
        }
    }
</script>

<style scoped>
    div {
        display: block;
        background: #f5f5f5;
        position: fixed;
        height: calc(100% - 8rem);
        width: 100%;
    }
</style>