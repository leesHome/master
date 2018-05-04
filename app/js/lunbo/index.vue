<template>
    <section :class="cname">
        <swiper :options="options" :not-next-tick="options.notNextTick">
            <swiper-slide v-for="item in items" :key="item.href">
                <router-link :to="{ name: item.href}">
                    <img :src="item.src" alt="">
                </router-link>
            </swiper-slide>
            <div class="swiper-pagination" v-if="options.pagination" slot="pagination"/>
        </swiper>
        <Lists></Lists>
    </section>
</template>

<script>
    import {swiper, swiperSlide} from 'vue-awesome-swiper'
    import Lists from '../common/lists/list'
    export default {
        name: "index",
        components: {
            swiper,
            swiperSlide,
            Lists
        },
        props: {
            cname: {
                type: String,
                default: ""
            },
            options: {
                type: Object,
                default() {
                    return {
                        autoplay: true,
                        loop: true,
                        pagination: {
                            el: ".swiper-pagination",
                        },
                        notNextTick: false,
                    }
                }
            },
            items: {
                type: Array,
                default() {
                    return [
                        {
                            'href': '#/',
                            'src': 'http://img12.360buyimg.com/jrpmobile/jfs/t13465/324/2563794460/43029/3ffca963/5a421f83Ne8089231.jpg?width=750&height=320'
                        }, {
                            'href': '#/',
                            'src': 'http://img12.360buyimg.com/jrpmobile/jfs/t13744/11/2508939408/43213/58bfe502/5a421ff3N52d0a474.jpg?width=750&height=320'
                        }, {
                            'href': '#/',
                            'src': 'http://img12.360buyimg.com/jrpmobile/jfs/t16138/325/817844900/36681/5d874455/5a422029Ncd678ea3.jpg?width=750&height=320'
                        }, {
                            'href': '#/',
                            'src': 'http://img12.360buyimg.com/jrpmobile/jfs/t13744/11/2508939408/43213/58bfe502/5a421ff3N52d0a474.jpg?width=750&height=320'
                        }
                    ]
                }
            }
        }
    }
</script>

<!--
<style lang="scss" scoped>
    .swiper {
        margin: 10px auto;
        width: 100%;
        height: 30rem;
        overflow: hidden;
        .swiper-slide {
            width: 100%;
            height: 6.4rem;
            &.swiper-slide-active {
                img {
                    margin-top: 0;
                    width: 100%;
                    height: 100%;
                }
            }
            img {
                display: block;
                margin: 0 auto;
                margin-top: 3.5%;
                width: 90.625%;
                height: 90.625%;
                vertical-align: middle;
                -webkit-transition: all 1s ease 0s;
                -moz-transition: all 1s ease 0s;
                -ms-transition: all 1s ease 0s;
                -o-transition: all 1s ease 0s;
                transition: all 1s ease 0s;
            }
        }
    }

</style>-->
<style lang="css">
    @import "~swiper/dist/css/swiper.css";
    section {
        margin: 1rem auto;
    }
    section img {
        width: 100%;
    }
</style>
