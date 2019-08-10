<template>
   <div>
     <input type="button" :value="msg" @click="numberChanged">{{ msg }}</input>
      <p>{{ msg }}</p>
   </div>
</template>

<script>
export default {
  props: ['msg'],
  data() {
    return {
      message: '',
      msg: 0
    }
  },
  mounted:function(){
    this.msg = localStorage.cli;
    this.msg = ++this.msg;
  },
  methods: {
    changeMessage(event) {
      this.message = event.target.value;
      this.$emit('messageChanged', this.message);
    },
    numberChanged(event) {
      if (localStorage.cli) {
         localStorage.cli = ++localStorage.cli;
       } else{
         localStorage.cli = 1;
       }
      this.number = ++this.number;
      this.number = localStorage.cli;
      alert(localStorage.cli);
      this.$emit('numberChanged', this.number);
    },
  }
}
</script>

<style lang="css" scoped>
</style>
