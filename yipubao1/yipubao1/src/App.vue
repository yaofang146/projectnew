<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
html,body{
  width:100%;
  height:100%;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* font-size:12px; */
  height:100%;
}

*{
  padding:0;
  margin:0;
}
a{
  text-decoration:none;
}
li{
  list-style:none;
}
/*媒体查询*/
@media screen and (min-width:321px) and (max-width:375px) {
    html {
        font-size: 11px;
    }
}

@media screen and (min-width:376px) and (max-width:414px) {
    html {
        font-size: 12px;
    }
}
@media screen and (min-width:415px) and (max-width:639px) {
    html {
        font-size: 15px;
    }
}
@media screen and (min-width:640px) and (max-width:719px) {
    html {
        font-size: 20px;
    }
}
@media screen and (min-width:720px) and (max-width:749px) {
    html {
        font-size: 22.5px;
    }
}
@media screen and (min-width:750px) and (max-width:799px) {
    html {
        font-size: 23.5px;
    }
}





@font-face {font-family: "iconfont";
  src: url('//at.alicdn.com/t/font_942188_vtfctnewebr.eot?t=1544495877791'); /* IE9*/
  src: url('//at.alicdn.com/t/font_942188_vtfctnewebr.eot?t=1544495877791#iefix') format('embedded-opentype'), /* IE6-IE8 */
  url('data:application/x-font-woff;charset=utf-8;base64,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') format('woff'),
  url('//at.alicdn.com/t/font_942188_vtfctnewebr.ttf?t=1544495877791') format('truetype'), /* chrome, firefox, opera, Safari, Android, iOS 4.2+*/
  url('//at.alicdn.com/t/font_942188_vtfctnewebr.svg?t=1544495877791#iconfont') format('svg'); /* iOS 4.1- */
}

.iconfont {
  font-family:"iconfont" !important;
  font-size:16px;
  font-style:normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.icon-zhu:before { content: "\e671"; }

.icon-ai59:before { content: "\e6b1"; }

.icon-tel:before { content: "\e641"; }

.icon-guidepost:before { content: "\e602"; }

.icon-suo:before { content: "\e657"; }

.icon-wei-:before { content: "\e605"; }

.icon-yongjin:before { content: "\e66d"; }

.icon-dianhua:before { content: "\e61b"; }

.icon-duigou:before { content: "\e611"; }

.icon-kehu1:before { content: "\e66c"; }

.icon-kehu:before { content: "\e600"; }

.icon-personal-card:before { content: "\e606"; }

.icon-fenxiang:before { content: "\e60b"; }

.icon-wodehaoyou:before { content: "\e64f"; }

.icon-qicheqianlian-:before { content: "\e603"; }

.icon-wo:before { content: "\e685"; }

.icon-quanyou:before { content: "\e608"; }

.icon-index:before { content: "\e601"; }

.icon-feiji:before { content: "\e604"; }

.icon-shezhi:before { content: "\e607"; }

.icon-ziyuanldpi:before { content: "\e613"; }


</style>
