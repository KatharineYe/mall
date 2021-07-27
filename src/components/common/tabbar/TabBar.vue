<template>
  <div id='tab-bar'>
    <slot></slot>
  </div>
</template>

<script>
export default {
  name: 'TabBar',
  data () {
    return {
    }
  },
  methods: {
  },
  computed: {
  },
  components: {
  }
}
</script>

<style scoped>
#tab-bar {
  display: flex;
  background: rgba(174, 175, 174, 0.925);

  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;

  text-align: center;
}
</style>

