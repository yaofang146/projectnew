<template>
  <div class="logon">
    <div class="title">
      <img src="../assets/0.jpg" />
      <div class="word">
        <p>易铺宝</p>
        <p>国内仅有的地产众销平台</p>
      </div>
    </div>
    <div class="logon_content">
      <div class="tel">
        <i class="iconfont icon-tel"></i>
        <input type="text" placeholder="请输入手机号码" />
      </div>
      <div class="password">
        <i class="iconfont icon-suo"></i>
        <input type="text" placeholder="请输入6-8位密码" />
        <span class="pointer">忘记密码？</span>
      </div>
      <div class="regist pointer">注册</div>
      <div class="logon-button pointer" >登陆</div>
    </div>
    <div class="powered">
      Powered by xxx
    </div>
  </div>
</template>

<script>
export default {
  name: 'Logon',
  data () {
    return {
      msg: ''
    }
  },
  components:{},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div.logon div.title{
  margin:0 auto;
  position:relative;
}

div.word{
  position:absolute;
  top:50px;
  left:50px;
  text-align:left;
  color:#fff;
  font-size:15px;
}
div.word p:first-child{
  font-size:24px;
  margin-bottom:20px;
}
div.logon div.logon_content{
  margin:30px auto 0;
  text-align: left;
  padding:20px;
}
div.logon div.logon_content i{
    font-size:30px;
    margin:0 50px 0 0;
    color:#c80039;
}
div.logon div.logon_content input{
    font-size:18px;
    width:140px;
    border:0;
    color:#e5e5e5;
    outline: none;
}
div.logon div.logon_content div.tel,div.logon div.logon_content div.password{
  padding-bottom:20px;
  border-bottom:1px solid #c80039;
  margin-bottom:40px;
  display:flex;
}
div.password span{
  color:#c80039;
  font-size:18px;
  margin-left:10px;
  line-height: 33px;
}
div.regist{
  font-size:18px;
  color:#c80039;
  display:inline;
  border-bottom:1px solid #c80039; 
}
div.logon-button{
  width:300px;
  height:48px;
  background:#c80039;
  color:#fff;
  line-height:48px;
  font-size:20px;
  margin:40px auto;
  text-align:center;
}
div.powered{
  font-size:16px;
  color:#c80039;
}
.pointer{
  cursor:pointer;
}



</style>
