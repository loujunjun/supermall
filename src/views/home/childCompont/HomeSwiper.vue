<template>
  <div class="home-swiper">
    <swiper>
      <swiper-item v-for="item in cbanner">
        <a  :href="item.link">
          <img :src="item.image" alt=""/>
        </a>
      </swiper-item>
    </swiper>
  </div>
</template>

<script>
  import {Swiper,SwiperItem} from 'components/common/swiper/index'
  export default {
    name: "HomeSwiper",
    props:{
        cbanner:{
          type:Array,
          default(){
            return []
          }
        }
    },
    components:{
      Swiper,
      SwiperItem
    },
    created(){
      // console.log(this.cbanner)
    }
  }
</script>

<style scoped>

</style>
