<template>
  <div>
    <Header title="我的喵喵"></Header>
    <TabBar></TabBar>
  </div>
</template>

<script>

import Header from '../../components/Header/index';
import TabBar from '../../components/TabBar/index';

export default {
  name:'Mine',
  components:{
    Header,
    TabBar
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