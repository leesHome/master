<template>
    <section class="wrapCom">
        <ul class="nav">
            <li class="comNav">
                <router-link :to="{ name: 'home'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t3991/64/2521945388/12110/93c0139/58d1e462Ncf294123.png?width=132&height=132" alt="">
                    <p>优惠券</p>
                </router-link>
            </li>
            <li class="comNav">
                <router-link :to="{ name: 'money'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t5590/252/875247023/17343/946aa72c/59224650N0f7ffc92.png?width=132&height=132" alt="">
                    <p>领红包</p>
                </router-link>
            </li>
            <li class="comNav">
                <router-link :to="{ name: 'ious'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t4393/329/2180608902/13217/c88c0cec/58ec9dcdN1534e2d7.png?width=132&height=132" alt="">
                    <p>抢钢镚</p>
                </router-link>
            </li>
            <li class="comNav">
                <router-link :to="{ name: 'raise'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t4618/115/2179710654/11347/bf520df/58ec9d84Nfd169001.png?width=132&height=132" alt="">
                    <p>领京豆</p>
                </router-link>
            </li>
            <li class="comNav">
                <router-link :to="{ name: 'home'}">
                    <img src="//img12.360buyimg.com/jrpmobile/jfs/t5488/298/1036263348/12073/b4f4de97/590ac8e8Ne9def22e.png?width=135&height=135" alt="">
                    <p>白条提额</p>
                </router-link>
            </li>
        </ul>
    </section>
</template>

<script>
    export default {
        name: "list"
    }
</script>

<style scoped lang="scss">
    .wrapCom{
        width: 100%;
        height: 5rem;
        .nav{
            margin: 0;
            padding: 0;
            display: flex;
            text-align: center;
            .comNav{
                width: 20%;
                height: 5rem;
                img{
                    display: inline-block;
                    width: 3rem;
                    margin-bottom:  0.4rem;
                }
                p{
                    color: #656565;
                    &:hover{
                        color: red;
                    }
                }
            }
        }
    }
</style>