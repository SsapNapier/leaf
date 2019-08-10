<template>
  <div>
     <message :msg="number"  @numberChanged="number = $event"></message>
   <!-- <h1>{{ message }}</h1> -->
       <appinput :msg="number"  @numberChanged="number = $event"></appinput>
  </div>
</template>

<script>
const NUMBER = "number"
import appinput from '~/components/input.vue'
import message from '~/components/Message.vue'
export default {
  data() {
    return {
      message: 'This is a great Message',
      number: 0
    }
  },
  components: {
    appinput,
    message
  }
}
</script>

<style lang="sass" scoped>
</style>
