<template>
  <a-button type="primary" @click="clickPrimary">Primary Button</a-button>
</template>

<script>
export default {
  name: 'ButtonNormal',
  methods: {
    clickPrimary () {
      console.log('clickPrimary')
    }
  }
}
</script>
<style scoped></style>
