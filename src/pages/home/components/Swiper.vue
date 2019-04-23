<template>
  <div class="wrapper">
    <swiper :options="swiperOption">
      <!-- slides -->
      <swiper-slide v-for="item of swiperList" :key="item.id">
        <img class="swiper-img" :src="item.imgUrl">
      </swiper-slide>

      <!-- Optional controls -->
      <div class="swiper-pagination"  slot="pagination"></div>

    </swiper>
  </div>

</template>

<script>
    export default {
        name: "HomeSwiper",
        data() {
          return {
            swiperOption:{
              pagination:{
                el:'.swiper-pagination',
              },
              loop:true,
              autoplay:true
            },
            swiperList:[{
              id:'0001',
              imgUrl:'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20194/9f39c398e63315d7375efd08028f040e.jpg_750x200_4f536dd8.jpg'
            },{
              id:'0002',
              imgUrl:'http://mp-piao-admincp.qunarzz.com/mp_piao_admin_mp_piao_admin/admin/20194/cda2a455558c82c25f972c647c273289.jpg_750x200_701e05e2.jpg'
            }]
          }
        },
    }
</script>

<style scoped lang="stylus">
  .wrapper>>>.swiper-pagination-bullet-active
    background #ffffff !important
  .wrapper
    overflow: hidden
    width 100%
    height 0
    padding-bottom 27%
    background #eee
    .swiper-img
      width 100%

</style>
