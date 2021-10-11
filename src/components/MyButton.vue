<template>
  <div>
    <button @click="onClick">Click me (v2)</button>
    <h2>Click count v2 {{ clickCount }}</h2>
  </div>
</template>
<script lang="ts">
import { ref, defineComponent } from "vue-demi";

export default defineComponent({
  name: "MyButton",
  props: {},
  setup() {
    const clickCount = ref(0);
    const onClick = () => {
      clickCount.value += 1;
    };

    return { onClick, clickCount };
  },
});
</script>
