<template>
  <div>
    <button @click="sendMessage">Send Data from Child 1</button>
  </div>
</template>

<script>
export default {
  methods: {
    sendMessage() {
      this.$emit('sendData', 'Data from Child 1');
    }
  }
};
</script>
