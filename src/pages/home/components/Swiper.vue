<template>
    <div class="wrapper">
        <swiper :options="swiperOption">
            <!-- slides -->
            <swiper-slide v-for="item in swiperList" :key="item.id">
                <img class="swiper-img" :src="item.imgUrl">
            </swiper-slide>
            <div class="swiper-pagination" slot="pagination"></div>
        </swiper>
    </div>
</template>

<script>
export default {
  name: 'HomeSwiper',
  data () {
    return {
      swiperOption: {
        pagination: {
          el: '.swiper-pagination',
          type: 'bullets'
        },
        autoplay: {
          delay: 3000,
          stopOnLastSlide: false,
          disableOnInteraction: false
        },
        loop: true
      },
      swiperList: [
        {
          id: '001',
          imgUrl: 'https://m.360buyimg.com/mobilecms/s750x366_jfs/t1/19191/22/7682/132635/5c6f5d99Ebfa1045f/26616ded19a81661.jpg!cr_1125x549_0_72!q70.jpg.dpg'
        },
        {
          id: '002',
          imgUrl: 'https://m.360buyimg.com/mobilecms/s750x366_jfs/t1/30821/27/3649/76610/5c774e25E3dda7c39/6b9f2c7547c29cea.jpg!cr_1125x549_0_72!q70.jpg.dpg'
        },
        {
          id: '003',
          imgUrl: 'https://m.360buyimg.com/mobilecms/s750x366_jfs/t1/18179/5/8793/99013/5c795292E3e1dba85/12e9c3a346839327.jpg!cr_1125x549_0_72!q70.jpg.dpg'
        },
        {
          id: '004',
          imgUrl: 'https://m.360buyimg.com/mobilecms/s750x366_jfs/t1/30782/16/4549/134502/5c7e5c15Ee1e93de0/e2ad2b15ad53bf64.jpg!cr_1125x549_0_72!q70.jpg.dpg'
        },
        {
          id: '005',
          imgUrl: 'https://m.360buyimg.com/mobilecms/s750x366_jfs/t1/30044/35/4497/90390/5c7dd479Ef7897abc/b97cde862607823c.jpg!cr_1125x549_0_72!q70.jpg.dpg'
        }
      ]
    }
  }
}
</script>

<style lang="stylus" scoped>
  .wrapper >>> .swiper-pagination-bullet-active
    background-color: #fff
  .wrapper
    overflow: hidden
    width: 100%
    height: 0
    padding-bottom: 48.8%
    .swiper-img
      width: 100%
</style>
