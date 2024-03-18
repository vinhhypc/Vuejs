<template>
  <div class="cover">
    <ButtonNormal ref="buttonref"/>
    <button @click="onClick">Click me</button>
    <modal-component/>
  </div>
  
</template>

<script>
import ButtonNormal from '~/components/ButtonNormal/ButtonNormal.vue'
import ModalComponent from '~/components/Modal/ModalComponent.vue'

export default {
  components: { ButtonNormal, ModalComponent },
  methods: {
    onClick() {
     console.log(this.$refs.buttonref) 
    }
  }
}

</script>

<style>
.cover{
  margin-top: 20px;
}
</style>