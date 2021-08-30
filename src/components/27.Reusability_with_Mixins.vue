<template>
  <div>
    <button @click="incrementCount">Clicked {{ count }} times</button>
  </div>
</template>

<script>

//50.Reusability with Mixins -

import CounterMixin from "../../27.mixins/counter"

export default {
  name: "ClickCounter",
  mixins: [CounterMixin],
  data() {
    return {
      count: 100,
    };
  },
  // methods: {
  //   incrementCount() {
  //     this.count += 1;
  //   },
  // },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
