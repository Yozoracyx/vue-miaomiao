<template>
  <div class="wrapper" ref="wrapper">
    <slot></slot>
  </div>
</template>

<script>
// 弹性滑动
import BScroll from "better-scroll";

export default {
  name: "Scroller",
  components: {},
  props: {
    handleToSrcoll: {
      type: Function,
      default: function() {}
    },
    handleToTouchEnd: {
      type: Function,
      default: function() {}
    }
  },
  data() {
    return {
    };
  },
  mounted() {
    var scroll = new BScroll(this.$refs.wrapper, {
      tap: true,
      probeType: 1
    });

    this.scroll = scroll;

    scroll.on("scroll", pos => {
      this.handleToSrcoll(pos);
    });

    scroll.on("touchEnd", pos => {
      this.handleToTouchEnd(pos);
    });
  },
  methods: {
    toScrollTop(y) {
      this.scroll.scrollTo(0, y);
    }
  }
};
</script>
<style lang="scss" scoped>
.wrapper {
  height: 100%;
}
</style>