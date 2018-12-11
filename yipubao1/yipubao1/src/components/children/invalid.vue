<template>
  <div class="invalid">
    <ul>
      <li v-for="set in sets" :key="set.id">
        <div class="msg">
          <div><span>{{set.name}}</span></div>
          <div><span>{{set.phone}}</span></div>
          <div><i class="iconfont icon-dianhua"></i></div>
        </div>
        <div class="project"><span>推荐项目：</span><span>{{set.project}}</span></div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'invalid',
  data () {
    return {
      sets:[
        {id:1,name:'孙露',phone:18432343978,project:'万毒项目'},
        {id:2,name:'商铺',phone:18432343978,project:'金叶别墅'},
        {id:3,name:'看出',phone:18432343978,project:'乐都供应'},
        {id:4,name:'看出',phone:18432343978,project:'乐都供应'},
        {id:5,name:'看出',phone:18432343978,project:'乐都供应'},
        {id:6,name:'看出',phone:18432343978,project:'乐都供应'},
      ]
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div.customer{
  padding:0;
}
div.invalid{
  flex-grow: 1;
  padding: 0;
}
.invalid ul{
  width:100%;
  overflow: scroll;
}
li{
  margin-bottom: 1.417rem;
  border-top:1px solid #f0e9e9;
}
div.msg{
  color:#e21a31;
  font-size:1.25rem;
  display: flex;
  background: #fff;
}
div.phone{
  color:#aaa;
}
div.project{
  color:#fff;
  background:#e21a31;
  text-align: left;
  padding-left: 2rem;
}
.msg div:first-child{
  width:7.7rem;
  padding:1.083rem 0;
  border-right: 1px solid #e21a31;
    margin: 1rem 0;
}
.msg div:nth-child(2){
  /* width:11.33rem; */
    flex-grow: 1;
  padding:2.083rem 0.583rem 2.417rem 4.17rem;
}
.msg div:nth-child(3){
  background: #f5f5f5;
  width:5.67rem;
  padding:2.17rem 1.83rem 2.3rem 1.83rem;
}
.msg div:nth-child(3) i{
  font-size:1.583rem;
}
div.project span{
  font-size: 1rem;
  display: inline-block;
  padding:0.583rem 0;
}
</style>