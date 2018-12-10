<template>
<div>
    <ul>
        <li  v-for="item in items" v-bind:key="item.id">
            <div class="title">
                <div class="img"><img src="../../assets/1.jpg" /></div>
                <div class="content">
                    <h2>{{item.title}}</h2>
                    <div>
                        <p><span>地址</span><span>{{item.address}}</span></p>
                        <p><span>均价</span><span>{{item.price}}元/㎡</span></p>
                    </div>
                </div>
            </div>
            <div class="reward"><p>推荐奖励：成交额10%</p></div>
        </li>
    </ul>
</div>

</template>
<script>
export default {
    name:'project',
    data(){
        return{
            items:[
                    {id:1,title:'万都项目',address:'高新管委会附近',price:12000,},
                    {id:2,title:'万都项目',address:'高新管委会附近',price:12000,},
                    {id:3,title:'万都项目',address:'高新管委会附近',price:12000,},
                    {id:4,title:'万都项目',address:'高新管委会附近',price:12000,},
                    {id:5,title:'万都项目',address:'高新管委会附近',price:12000,},
                ],  
            
        }
    },
    components:{}
}

</script>
<style scoped>
div.title{
    display:flex;
}
div.title .img{
    width:35.4%;
    height:100%;
    padding: 0 5%;
}
.img img{
    width: auto;
    height: auto;
    max-width: 100%;
    max-height: 100%;
    float:left;
    overflow: hidden;
}
div.title div.content{
    flex-grow: 1;
    text-align: left;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding-top: 10px;
}
div.content h2{
    color:#e21a31;
    font-size:0.63rem;
}
div.reward{
    text-align: left;
    padding: 2% 5%;
    color:#e21a31;
}
li{
    margin-bottom: 9px;
    box-shadow: 0 3px 3px #ccc;
}
li:last-child{
    box-shadow:0 0;
}
div.content div p span:first-child{
    margin-right:1.67rem;
}
</style>