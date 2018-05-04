<template lang="html">
    <div class="act">
        <Headers></Headers>
        <Contexts></Contexts>
        <Navs></Navs>
    </div>
</template>

<script>
    import Headers from '../common/header/index';
    import Navs from '../common/nav/index';
    import Contexts from '../context/index';
    export default {
        name: 'home',
        components: {
            Headers,
            Contexts,
            Navs
        }
    }
</script>

<style lang="scss" module>
    @import '../../css/reset.scss';
    .act{
        color: red;
    }
</style>
