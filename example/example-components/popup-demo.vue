<template>
  <div class="demo">
    <wmui-popup 
    v-model="showPopup1" 
    position="bottom" 
    cover="30%"

    @maskClick="showPopup1 = false">
    <p>hello</p>
    </wmui-popup>
    
    <wmui-popup 
    v-model="showPopup2" 
    position="left"
    cover="30%" 
    @maskClick="maskClick"
    @click.native="showPopup2 = false">
    </wmui-popup>

    <wmui-popup 
    v-model="showPopup3" 
    position="left" 
    cover="30%"
    @click.native="showPopup3 = false"
    :mask="false">
    </wmui-popup>


    <wmui-button @click.native="showPopup1 = true">点击mask关闭</wmui-button>
    <wmui-button @click.native="showPopup2 = true">点击popup关闭</wmui-button>
    <wmui-button @click.native="showPopup3 = true">关闭mask显示</wmui-button>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        showPopup1: false,
        showPopup2: false,
        showPopup3: false
      }
    },
    methods: {
      maskClick () {
        alert('你点击了mask')
      }
    }
  }
</script>

