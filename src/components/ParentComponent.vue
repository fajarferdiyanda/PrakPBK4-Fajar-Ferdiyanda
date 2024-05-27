<template>
  <div>
    <h1>Parent Component</h1>
    <p>Data from children: {{ message }}</p>
    <ChildComponent1 @sendData="handleData" />
    <ChildComponent2 @sendData="handleData" />
    <SlotComponent>
      <template v-slot:default>
        <p>This is a slot content from parent</p>
      </template>
    </SlotComponent>
  </div>
</template>

<script>
import ChildComponent1 from './ChildComponent1.vue';
import ChildComponent2 from './ChildComponent2.vue';
import SlotComponent from './SlotComponent.vue';

export default {
  components: {
    ChildComponent1,
    ChildComponent2,
    SlotComponent
  },
  data() {
    return {
      message: ''
    };
  },
  methods: {
    handleData(data) {
      this.message = data;
    }
  }
};
</script>
