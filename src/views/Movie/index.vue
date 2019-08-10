<template>
  <div>
    <Header title="喵喵电影"></Header>
    <TabBar></TabBar>
  </div>
</template>

<script>

import Header from '../../components/Header/index';
import TabBar from '../../components/TabBar/index';

export default {
  name:'Movie',
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