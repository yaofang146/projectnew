<template>
  <div class="customer">
    <div>
      <span>进行中</span>
      <span>无效</span>
    </div>
    <router-view/>
  </div>
  
</template>

<script>
import message from '@/components/children/message'
import invalid from '@/components/children/invalid'

export default {
  name: 'customer',
  data () {
    return {
      
    }
  },
  components:{message,invalid},
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
div.customer{
  /* padding:0 1.33rem; */
  height:100%;
  background:#f5f5f5;
  display: flex;
  flex-direction: column;
}
.customer div{
  display:flex;
  justify-content: space-between;
  padding:1.5rem 1.417rem;
}
.customer div:first-child{
    padding: 1.5rem 2.747rem 2rem;

}
span{
  border-radius: 5px;
  color:#e21a31;
  background:#fff;
  border:1px solid #e21a31;
  font-size:1rem;
  width:9rem;
  padding:0.67rem;
  line-height: 100%;
  height: 100%;
  }
span:first-child{
  color:#fff;
  background:#e21a31;
}
</style>