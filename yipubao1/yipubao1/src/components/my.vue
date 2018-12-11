<template>
    <div class="myfriend">
        <div class="information">
            <div class="card">
                <div class="icon"><i class="iconfont icon-ai59"></i><span>{{name}}</span></div>
                <div class="msg">
                    <div class="bankcard">
                        <span>{{bankcard}}</span>
                        <i class="iconfont icon-shezhi"></i>
                    </div>
                    <div class="phone">
                        <i class="iconfont icon-dianhua"></i>
                        <span>联系电话：</span>
                        <span>{{phone}}</span>
                    </div>
                    <div class="money">
                        <i class="iconfont icon-yongjin"></i>
                        <span>累计佣金：</span>
                        <span>{{money}}</span>
                    </div>
                </div>
            </div>
            <div class="menu">
                <span>待提现</span>
                <span>已提现</span>
                <span>已到账</span>
            </div>
        </div>
        <div class="list">
            <ul>
                <li v-for="item in items" :key="item.id">
                    <i class="iconfont" v-bind:class="item.icon"></i>
                    <span>{{item.title}}</span>
                    <i class="iconfont icon-quanyou"></i>
                </li>
            </ul>
        </div>
    </div>
  
</template>

<script>
export default {
  name: 'myfriend',
  data () {
    return {
      items:[
          {id:1,title:'我的佣金',icon:'icon-yongjin'},
          {id:2,title:'我的名片',icon:'icon-personal-card'},
          {id:3,title:'分享给朋友',icon:'icon-fenxiang'},
          {id:4,title:'我的好友',icon:'icon-wodehaoyou'},
      ],
      bankcard:'已绑银行卡',
      name:'孙露',
      phone:18625364675,
      money:4000,
    }
  },
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div.myfriend{
    height:100%;
    display:flex;
    flex-direction: column;
}
div.information{
    width:100%;
}
div.card{
    border-bottom:1px solid #ccc;
    display: flex;
}
div.icon{
    border-right:1px solid #f00;
    padding: 0 1.83rem 0 1.67rem;
    margin: 0.83rem 0 0.583rem 0;
}
div.icon i{
    display: block;
    color:#aaa;
    font-size: 4.33rem;
}
div.icon span{
    color:#f00;
    font-size: 1.083rem;
}
div.msg{
    padding:1.083rem 1.333rem 1.167rem 1rem;
    width: 100%;
    text-align: left;
}
div.bankcard{
    margin-bottom:0.83rem;
}
div.phone{
    margin-bottom:0.53rem;
}
div.msg i{
    font-size: 1.5rem;
    color:#f00;
}
div.bankcard{
    display: flex;
    justify-content: space-between;
}
div.bankcard span{
    background:#f00;
    color:#fff;
    font-size:1rem;
    width:6.75rem;
    border-radius: 5px;
    text-align: center;
    padding:0.5rem 0;
}
div.bankcard i{
    color:#aaa;
}
div.phone i,div.money i{
    margin-right:1.083rem;
}
div.menu{
    display:flex;
    justify-content: space-between;
    padding:1.2rem 1.3rem;

}
div.menu span{
    color:#f00;
    background:#fff;
    padding:0.67rem 0;
    font-size: 0.917rem;
    border:1px solid #f00;
    width:6rem;
    border-radius: 5px;
}
div.list{
    background:#f5f5f5;
    width:100%;
    flex-grow: 1;
}
.list ul{
    padding:0.67rem 1.33rem 2rem 1.33rem;
}
.list ul li{
    padding:1rem;
    color:#f00;
    font-size:0.917rem;
    border-radius: 5px;
    box-shadow: 0 5px 0 #f00;
    background:#fff;
    margin-bottom: 1.83rem;
    display:flex;
    justify-content: space-between;
}
.list ul li i:first-child{
    font-size:2.33rem;
}
.list ul li span{
    color:#000;
    line-height:2.5rem;
    margin-left: -19rem;
}
.list ul li i:last-child{
    line-height:2.4rem;
}
</style>