<template>
  <transition name="wmui-animation-fade">
    <div class="wmui-mask" v-if="show" @click="handleClick" :style="maskStyle"></div>
  </transition>
</template>
<script>
export default {
  name: 'wmui-mask',
  props: {
    show: {
      type: Boolean,
      default: false
    },
    opacity: {
      type: Number,
      default: 0.4
    },
    zIndex: { // mask层级
      type: Number
    },
    onClick: { // 点击mask
      type: Function
    }
  },
  methods: {
    handleClick() {
      if (this.onClick) {
        this.onClick()
      }
    }
  },
  computed: {
    maskStyle() {
      return {
        'opacity': this.opacity,
        'z-index': this.zIndex
      }
    }
  }
}
</script>

