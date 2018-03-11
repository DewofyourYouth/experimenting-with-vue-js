<template>
  <div>
      <p>{{msg}}</p>
      <input type="text" :value="msg" @input="changeMessage">
  </div>
</template>

<script>
    export default{
        props: ['msg'],
        data() {
            return {
                message: ''
            }
        },
        methods: {
            changeMessage(event) {
                this.message = event.target.value;
                this.$emit('messageChanged', this.message);
            }
        }
    }
</script>
