# universal-button written in Vue2

## How to use it
- no BUILD! The component is published as NPM package in form of source code
- never import anything in this project from `vue` or `@vue/composition-api`, instead use `vue-demi`
- add dependency:
```
yarn add ladariha-button-2
```

- import vue file directly
```
import MyButton from "ladariha-button-2/src/components/MyButton.vue";
```
## Sample usage in Vue3 project:

```
<template>
  <div id="app">
    <MyButton />
    Reactive number: {{ randomNumber }}
  </div>
</template>

<script lang="ts">
import MyButton from "ladariha-button/src/components/MyButton.vue";
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "App",
  components: {
    MyButton,
  },
  setup() {
    const randomNumber = ref(Math.random());

    setInterval(() => {
      randomNumber.value = Math.random();
    }, 3000);

    return { randomNumber };
  },
});
</script>
```
