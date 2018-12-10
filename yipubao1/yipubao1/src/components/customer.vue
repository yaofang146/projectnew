<template>
  <div class="customer">
    <div>
      <span>进行中</span>
      <span>无效</span>
    </div>
    <!-- <router-link :to="{path:'./children/message'}"></router-link> -->
  </div>
  
</template>

<script>
import message from '@/components/children/message'
export default {
  name: 'customer',
  data () {
    return {
      
    }
  },
  components:{message},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.customer div{
  display:flex;
  justify-content: space-between;
}
span{
  border-radius: 5px;
  color:#f00;
  background:#fff;
  border:1px solid #f00;
}
span:first-child{
  color:#fff;
  background:#f00;
}
</style>