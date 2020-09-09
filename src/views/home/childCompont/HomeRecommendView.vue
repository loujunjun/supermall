<template>
  <div class="recommend">
    <div v-for="item in recommend" class="recommend-item">
      <a :href="item.link">
        <img :src="item.image"/>
        <div>{{item.title}}</div>
      </a>
    </div>
  </div>
</template>

<script>
  export default {
    name: "HomeRecommendView",
    props:{
      recommend:{
        type:Array,
        default(){
          return []
          }
        }
      },

    }

</script>

<style scoped>
  .recommend{
    display: flex;
    border-bottom:10px solid #eee;
    padding-bottom:20px ;
    font-size:13px;
  }
  .recommend-item{
    flex: 1;
    text-align: center;
  }
  .recommend-item img{
    width: 80%;
    margin: 10px 0;
  }
</style>
