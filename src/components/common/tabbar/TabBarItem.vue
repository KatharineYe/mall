<template>
  <div id='tab-bar-item' @click="itemClick">
    <div v-if='!isActive'><slot name='item-icon'></slot></div>
    <div v-else><slot name='item-icon-active'></slot></div>
    <div :style="activeStyle"><slot name='item-text'></slot></div>
  </div>
</template>


<script>
export default {
  name: 'TabBarItem',
  props: {
    path: String,
    activeColor: {
      type: String,
      default: '#d4237a'
    }
  },
  data () {
    return {
    }
  },
  methods: {
    itemClick() {
      if (!this.isActive) {
        this.$router.push(this.path); 
      }    
    }
  },
  computed: {
    isActive() {
      return this.$route.path.indexOf(this.path) !== -1;
    },
    activeStyle() {
      return this.isActive ? {color: this.activeColor} : {};
    }
  }
}
</script>

<style scoped>
#tab-bar-item {
  flex: 1;
  height: 49px;
  font-size: 14px;
}
#tab-bar-item img {
  height: 20px;
  width: 20px;
  margin-top: 5px;
  margin-bottom: 3px;
  vertical-align: middle;
}
</style>
