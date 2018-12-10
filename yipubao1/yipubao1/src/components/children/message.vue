<template>
  <div class="message">
    <ul>
      <li v-for="item in items" :key="item.id">
        <div class="msg">
          <div class="name">
            <span>{{item.name}}</span>
            <span>{{item.phone}}</span>
          </div>
          <div><i class="iconfont "></i></div>
        </div>
        <div class="project">
          <div>推荐项目：{{item.project}}</div>
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
      ]
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>