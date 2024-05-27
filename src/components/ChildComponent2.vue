<template>
  <div>
    <button @click="sendMessage">Send Data from Child 2</button>
  </div>
</template>

<script>
export default {
  methods: {
    sendMessage() {
      this.$emit('sendData', 'Data from Child 2');
    }
  }
};
</script>
