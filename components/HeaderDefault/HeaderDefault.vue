<template>
  <div class="header">
    <p>{{ text }}</p>
  </div>
</template>

<script>
export default {
  name: 'HeaderLayout',
  data () {
    return {
      text:'Header'
    }
  }
}
</script>
<style scoped>
.header {
  width: 100%;
  height: 60px;
  background: #1677ff;
  color: #fff;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
