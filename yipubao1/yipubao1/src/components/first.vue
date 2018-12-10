<template>
  <div class="first">
    <div class="customer">
        <div>
            <p>当前佣金</p>
            <p>￥{{money}}</p>
            <p>推荐客户</p>
        </div>
        <i class="iconfont icon-zhu"></i>
    </div>
    <div class="menu-in">
        <ul>
            <li>
                <i class="iconfont icon-kehu1"></i>
                <span>新客户</span>
                <span>{{number}}</span>
            </li>
            <li>
                <i class="iconfont icon-guidepost"></i>
                <span>跟进</span>
                <span>{{number}}</span>
            </li>
            <li>
                <i class="iconfont icon-feiji"></i>
                <span>到访</span>
                <span>{{number}}</span>
            </li>
            <li>
                <i class="iconfont icon-qicheqianlian-"></i>
                <span>认购</span>
                <span>{{number}}</span>
            </li>
            <li>
                <i class="iconfont icon-wei-"></i>
                <span>签约</span>
                <span>{{number}}</span>
            </li>
            <li>
                <i class="iconfont icon-ziyuanldpi"></i>
                <span>无效</span>
                <span>{{number}}</span>
            </li>
        </ul>
    </div>
    <div class="toggle-out">
        <div class="toggle">
            <div class="left">
                <span>西安</span>
            </div>
            <div class="right">
                <span>青岛</span>
            </div>
        </div>
    </div>
    <div class="introduce">
       <router-view></router-view> 
    </div>
  </div>
</template>

<script>
import project from '@/components/children/project'
export default {
  name: 'first',
  data () {
    return {
      money:5000,
      number:1
    }
  },
  components:{project},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div.first{
    height:100%;
    display:flex;
    flex-direction: column;
}

.customer{
    padding:4% 0 5% 0;
    background: #f5f5f5;
}
.customer div{
    border:2px solid #aaa;
    border-radius:50%;
    font-size:15px;
    width: 88px;
    margin: 0 auto;
    padding: 12px 0;
}
.customer div p:first-child{
font-size:15px;
transform: scale(0.8);
}
.customer div p:last-child{
font-size:15px;
transform: scale(0.9);
}
div.menu-in{
    flex-grow: 1;
    background: #f5f5f5;
}
div.menu-in ul{
    display:flex;
    flex-wrap: wrap;
}
div.menu-in ul li{
    position: relative;
    width:32.9%;
    padding: 12px 0;
    border: 1px solid #d1c7da;
}
div.menu-in ul li:nth-child(1){
    color:green;
    border-right:0;
    border-bottom:0;
    border-left:0;
}
div.menu-in ul li:nth-child(1) span:last-child{
    background: green;
    border:green;
}
div.menu-in ul li:nth-child(2){
    color:blue;
    border-right:0;
    border-bottom:0;
}
div.menu-in ul li:nth-child(2) span:last-child{
    background: blue;
    border:blue;
}
div.menu-in ul li:nth-child(3){
    color:yellow;
    border-bottom:0;
    border-right:0;
}
div.menu-in ul li:nth-child(31) span:last-child{
    background: yellow;
    border:yellow;
}
div.menu-in ul li:nth-child(4){
    color:orange;
    border-right:0;
    border-left:0;
}
div.menu-in ul li:nth-child(4) span:last-child{
    background: orange;
    border:orange;
}
div.menu-in ul li:nth-child(5){
    color:red;
    border-right:0;
}
div.menu-in ul li:nth-child(1) span:last-child{
    background: red;
    border:red;
}
div.menu-in ul li:nth-child(6){
    color:gray;
    border-right:0;
}
div.menu-in ul li:nth-child(6) span:last-child{
    background: gray;
    border:gray;
}
div.menu-in ul li i{
    display: block;
    font-size: 17px;
}
div.menu-in ul li span:nth-child(2){
    color:#ccc;
}
div.menu-in ul li span:last-child{
    position: absolute;
    right:25%;
    top:7%;
    border:1px solid #f00;
    border-radius:50%;
    background:#f00;
    width:15px;
    color:#fff;
}
div.introduce{
    margin:9px 0;
    overflow:scroll;
}
div.toggle-out{
    background: #f5f5f5;
}
div.toggle{
    width:20%;
    display:flex;
    justify-content: space-between;
    margin:10px auto;
}
div.left{
    border-bottom:0.5rem solid #f00;
    width:50%;
    height: 100%;
}
div.right{
    width:50%;
    border-bottom:0.5rem solid #ccc;
    height: 100%;
}
</style>
