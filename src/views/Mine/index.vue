<template>
  <div>
    <Header title="我的喵喵"></Header>
    <div id="content">
      <Login/>
    </div>
    <TabBar></TabBar>
  </div>
</template>

<script>

import Header from '../../components/Header/index';
import Login from '../../components/Login/index';
import TabBar from '../../components/TabBar/index';

export default {
  name:'Mine',
  components:{
    Header,
    TabBar,
    Login
  },
  props:{},
  data(){
    return {
    }
  },
  watch:{},
  computed:{},
  methods:{},
  created(){},
  mounted(){}
}
</script>
<style lang="scss" scoped>
</style>