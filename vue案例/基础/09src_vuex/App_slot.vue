<template>
  <div class="container"> 
    <Category title="游戏">
        <template slot-scope="{games}">
            <h2>{{games}}</h2>
            <ul>
              <li v-for="(item,index) in games" :key="index">{{item}}</li>
          </ul>
          Your Profile
        </template>    
    </Category>
  </div>
</template>
<script>
    import Category from './components/Category'
    export default {
      name: 'App',
      components:{Category},
      data() {
          return {
            foods:['火锅','烧烤','小龙虾','牛排'],
            // games:['红色警戒','穿越火线','劲舞团','超级玛丽'],
            films:['《教父》','《拆弹专家》','《你好，李焕英》','《尚硅谷》']
        }
      },
      methods: {

      },
    }
</script>

<style scoped>
    /* img{
      width: 100%;
    } */
    .footer,h4{
      text-align: center;
    }
    .footer a{
      margin: 0 5px;
    }
</style>