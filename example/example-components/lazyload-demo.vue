<template>
  <div class="demo">
    <div v-for="imgSrc in imgList" class="mb20">
      <wmui-lazyload :src="imgSrc"/>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      imgList: [
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg',
        'https://www.86886.wang/public/1520049901259.jpg'
      ]
    }
  }
}
</script>

