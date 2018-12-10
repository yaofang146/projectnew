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
  src: url('//at.alicdn.com/t/font_942188_rp41iwbeen9.eot?t=1543808335679'); /* IE9*/
  src: url('//at.alicdn.com/t/font_942188_rp41iwbeen9.eot?t=1543808335679#iefix') format('embedded-opentype'), /* IE6-IE8 */
  url('data:application/x-font-woff;charset=utf-8;base64,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') format('woff'),
  url('//at.alicdn.com/t/font_942188_rp41iwbeen9.ttf?t=1543808335679') format('truetype'), /* chrome, firefox, opera, Safari, Android, iOS 4.2+*/
  url('//at.alicdn.com/t/font_942188_rp41iwbeen9.svg?t=1543808335679#iconfont') format('svg'); /* iOS 4.1- */
}

.iconfont {
  font-family:"iconfont" !important;
  font-size:16px;
  font-style:normal;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.icon-zhu:before { content: "\e671"; }

.icon-tel:before { content: "\e641"; }

.icon-guidepost:before { content: "\e602"; }

.icon-suo:before { content: "\e657"; }

.icon-wei-:before { content: "\e605"; }

.icon-duigou:before { content: "\e611"; }

.icon-kehu1:before { content: "\e66c"; }

.icon-kehu:before { content: "\e600"; }

.icon-qicheqianlian-:before { content: "\e603"; }

.icon-wo:before { content: "\e685"; }

.icon-index:before { content: "\e601"; }

.icon-feiji:before { content: "\e604"; }

.icon-ziyuanldpi:before { content: "\e613"; }


</style>
