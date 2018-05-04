<template lang="html">
    <ul class="nav">
        <li class="comNav">
            <router-link :to="{ name: 'home'}">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3451/188/644771475/2428/800d7cb7/580f2435Nbfaa8055.png?width=66&height=66" alt="">
                <p>首页</p>
            </router-link>
        </li>
        <li class="comNav">
            <router-link :to="{ name: 'money'}">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3811/55/345433999/2930/116d3dd1/580f1e25N028a1f2c.png?width=66&height=66" alt="">
                <p>理财</p>
            </router-link>
        </li>
        <li class="comNav">
            <router-link :to="{ name: 'ious'}">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3343/179/621044750/1484/5af6b11a/580f50e4N005181d0.png?width=66&height=66" alt="">
                <p>白条</p>
            </router-link>
        </li>
        <li class="comNav">
            <router-link :to="{ name: 'raise'}">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3604/98/635506544/2317/443d3a51/580f240aNbee3dcc4.png?width=66&height=66" alt="">
                <p>众筹</p>
            </router-link>
        </li>
        <li class="comNav">
            <router-link :to="{ name: 'home'}">
                <img src="//img12.360buyimg.com/jrpmobile/jfs/t3340/68/639059082/2591/800e2d6b/580f51cdN4caf20b2.png?width=66&height=66" alt="">
                <p>我的</p>
            </router-link>
        </li>
    </ul>
</template>

<script>
    export default {
        name: 'nav'
    }
</script>

<style scoped lang="scss">
    .nav {
        width: 100%;
        height: 4rem;
        position: fixed;
        bottom: 0;
        box-sizing: border-box;
        display: flex;
        .comNav {
            text-align: center;
            width: 20%;
            float: left;
            a {
                height: 4rem;
                width: 100%;
                display: inline-block;
                overflow: hidden;
                img{
                    width: 1.5rem;
                    height: 1.5rem;
                    display: inline-block;
                    margin-top: 0.5rem;
                    margin-bottom:  0.4rem;
                }
                p{
                    font-size: 1.4rem;
                    color: #656565;
                    &:hover{
                            color: red;
                    }
                }
            }
            &:after{
                content: ".";
                display: block;
                height: 0;
                clear: both;
                visibility: hidden;
            }

        }
    }


</style>