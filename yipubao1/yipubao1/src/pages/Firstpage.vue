<template>
  <div class="firstpage">
    <div class="title"><h1>易铺宝</h1></div>
    <div class="section"><router-view/></div>
    <div class="menu">
      <ul>
        <li><i class="iconfont icon-index"></i>首页</li>
        <li><i class="iconfont icon-kehu"></i>客户</li>
        <li><i class="iconfont icon-wo"></i>我</li>
      </ul>
    </div>
  </div>
</template>

<script>
import first from '@/components/first'
import customer from '@/components/customer'
import myfriend from '@/components/my'

export default {
  name: 'Firstpage',
  data () {
    return {
      msg: ''
    }
  },
  components:{first,customer,myfriend},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div.firstpage{
  height:100%;
  display:flex;
  flex-direction: column;
}
div.title{
  color:#f00;
  font-size:1.25rem;
  padding: 11px 0;
  box-shadow: 0 5px 5px #ccc;
}
div.title h1{
  font-weight:normal;
  font-size: 1.25rem;
}
div.section{
flex-grow: 1;
 max-height: 86%;
overflow: hidden;
box-shadow: 0 5px 5px #ccc; 
display: flex;
flex-direction: column;
flex-basis: 0;
}
div.menu ul{
display:flex;
justify-content: space-around;
color:#ccc;
padding:12px 0;
}
ul li i{
  display: block;
  font-size:16px;
} 
</style>
