<template>
    <div class="wrapper" data-swiper-box>
        <swiper :options="swiperOption">
            <swiper-slide v-for="imgItem in swiperList" :key="imgItem.id">
                <img class="swiper-img" :src="imgItem.imgUrl" alt="">
            </swiper-slide>
            <div class="swiper-pagination"  slot="pagination"></div>
        </swiper>  
    </div>  
</template>

<script>
export default {
    name:'HomeSwiper',
    data () {
        return {
            swiperOption: {
                pagination: '.swiper-pagination',
                loop: true,
                autoplay: 2500,
            },
            swiperList:[{
                id: '0001',
                imgUrl:"https://img1.qunarzz.com/qs/1806/2f/1569f106565f8502.jpg"
            } , {
                id: "0002",
                imgUrl:"https://img1.qunarzz.com/qs/1806/b9/e50a5b23b6375d02.jpg"
            } , {
                id: "0003",
                imgUrl:"https://img1.qunarzz.com/qs/1806/5a/f96ab1ab02d30602.jpg"
            }]
        }
    }
}
</script>

<style lang="scss">
    div[data-swiper-box]{
        width: 100%;
        height: 0;
        overflow: hidden;
        padding-bottom: 25.6%;
        .swiper-pagination-bullet-active{
            background-color: #fff
        }
        .swiper-img{
            width: 100%;
        }
    }   
</style>
