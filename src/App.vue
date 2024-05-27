<template>
  <div id="app">
    <ParentComponent />
  </div>
</template>

<script>
import ParentComponent from './components/ParentComponent.vue';

export default {
  name: 'App',
  components: {
    ParentComponent
  }
};
</script>

<style>
body {
  background-color: rgb(0, 0, 255);
}
</style>
