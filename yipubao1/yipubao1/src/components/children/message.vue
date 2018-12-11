<template>
  <div class="message">
    <ul>
      <li v-for="item in items" :key="item.id">
        <div class="msg">
          <div class="name">
            <span>{{item.name}}</span>
            <span>{{item.phone}}</span>
          </div>
          <div><i class="iconfont icon-dianhua"></i></div>
        </div>
        <div class="project">
          <div>
            <span>推荐项目：{{item.project}}</span>
            <span>{{item.customer}}</span></div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'message',
  data () {
    return {
      items:[
        {id:1,name:'孙露',phone:18591954193,project:'万都项目',customer:'新客户'},
        {id:2,name:'孙露',phone:18591954193,project:'万都项目',customer:'新客户'},
        {id:3,name:'孙露',phone:18591954193,project:'万都项目',customer:'新客户'},
        {id:4,name:'孙露',phone:18591954193,project:'万都项目',customer:'新客户'},
        {id:5,name:'孙露',phone:18591954193,project:'万都项目',customer:'新客户'},
        {id:6,name:'孙露',phone:18591954193,project:'万都项目',customer:'新客户'},
        {id:7,name:'孙露',phone:18591954193,project:'万都项目',customer:'新客户'},
      ]
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div.customer{
  padding:0 1.33rem;}
div.message{
  height:100%;
  overflow:scroll;
}
div.message ul{
  display:flex;
  flex-direction: column;
  width:100%;
  height:100%;
}

div.msg{
  font-size:1.17rem;
  color:#f00;
  background:#fff;
  padding:0.83rem 1.25rem 0.83rem 1.5rem;
  display:flex;
  justify-content: space-between;
}
div.project{
font-size:0.917rem;
color:#555;
background:#f4f4f4;
padding:0.583rem 0.67rem 0.583rem 1.5rem;
}
li{
  box-shadow: 0 5px 5px #ccc;
  margin-bottom:0.917rem;
}
li:last-child{
  margin-bottom: 10rem;
}
.project div{
  display:flex;
  justify-content: space-between;
}
</style>