<template>
  <div class="regist">
    <div class="title">注册</div>
    <div class="content">
      <form action="" class="form-regist">
        <div class="form-group name">
          <label for="name">姓名：</label><input type="text" id="name" placeholder="请输入真实姓名" />
        </div>
        <div class="form-group tel">
          <label for="phone">电话：</label><input type="text" id="phone" placeholder="请输入手机号码" />
        </div>
        <div class="form-group code">
          <div><label for="code">验证码：</label><input type="text" id="code" /></div>
          <span class="code-span">获取验证码</span>
        </div>
        <div class="form-group password">
          <label for="password">密码：</label><input type="text" id="password" placeholder="请输入6-8位密码" />
        </div>
        <div class="form-group confirm">
          <label for="confirm">确认密码：</label><input type="text" id="confirm" placeholder="再次确认密码" />
        </div>
        <div class="form-group agree">
          <input type="checkbox" />
          我已阅读并同意<span>用户协议</span>
        </div>
        <div class="form-group regist-button">
          <a href="">注册</a>
        </div>
      </form>
      
    </div>
    <div class="powered">© Powered by xxx</div>
  </div>
</template>

<script>
export default {
  name: 'Regist',
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
.regist{
  height:100%;
  display:flex;
  flex-direction: column;
  padding:0 31px;
}
.title{
  font-size:15px;
  color:#ff0000;
  padding:15px 0 15px;
  text-align:center;
  margin-top:23px;
}
.content{
  flex-grow:1;
}
.powered{
  font-size:13px;
  padding:18px;
  text-align:center;
  color:#ff0000;
}
.form-group{
  font-size:11px;
  color:#ff0000;
  display:flex;
  padding:10px 0;
  border-bottom:1px solid #ff0000;
  margin-top:22px;
}
.agree,.regist-button{
  border-bottom:0;
}
.form-group label{
  width:25%;
  text-align:left;
}
.form-group input{
  flex-grow:1;
  border:0 none;
  margin-right:25%;
  text-align:center;
}
a{
  color:#f00;
  border-bottom: 1px solid #f00;
}
div.agree input{
  margin:0;
  flex-grow: 0;
}
div.agree{
  text-align: right;
  width:147px;
  margin:30px auto;
  color:#ccc;
}
div.agree span{
  color:#f00;
  text-decoration: underline;
}
.code-span{
  border:1px solid #f00;
  padding:5px 10px;
  line-height: 28px;
  border-radius: 5px;
}
div.code label{
  line-height:16px;
  padding: 7px 0 0 0;
}
div.code input{
  /* margin-right: 14%; */
  width:74%;
}
div.code{
  border:0;
  display:flex;
  justify-content: space-between;
}
div.code div{
  border-bottom:1px solid #f00;
  display:flex;
  width:73%;
}
/* div.regist{
    color:#c80039;
}
div.title{
  margin:20px auto;
}
div.content{
    padding:20px;

}
div.content div{
  display:flex;
  justify-content: space-between;
}
div.name,div.tel,div.code,div.password,div.confirm{
  padding-bottom:20px;
  border-bottom:1px solid #c80039;
  margin-bottom:30px;
}
div.code input{
  margin-right:-42px;
}
.code-span{
  border:1px solid #c80039;
  padding:5px;
  border-radius:3px;
  font-size:;
}
input{
  border:0 none;
  outline: none;
}
.regist-button{
  height:48px;
  background:#c80039;
  color:#fff;
  line-height:48px;
  font-size:22px;
  margin:30px auto;
  text-align:center;
}
.regist-button a{
  letter-spacing:1rem;
}
.regist-button span:first-child{
  margin-right:30px;
  margin-left:130px;
}
.regist-button span:last-child{
margin-right:130px;
}
div.agree{
  color:#ccc;
  font-size:12px;
  width:164px;
  margin:0 50px 0 auto;
}
 div.agree i{
  color:#c80039;
  font-size:14px;
  display:none;
}
div.agree input{
  width:20px;
  height:14px;
  margin:0;
  border:1px solid #ccc;
  margin:2px 0;
  overflow:visible;
}
div.agree span{
  color:#c80039;
  margin-right:10px;
} */
</style>
