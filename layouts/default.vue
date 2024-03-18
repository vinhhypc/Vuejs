<!-- default for all -->
<template>
  <div>
    <HeaderDefault />
    <Nuxt />
    <FooterLayout />
  </div>
</template>
<script>
import HeaderDefault from '~/components/HeaderDefault/HeaderDefault.vue'
import FooterLayout from '~/components/FooterDefault/FooterDefault.vue'
export default {
  name: 'DefaultLayout',
  components: { HeaderDefault, FooterLayout },
}
</script>
