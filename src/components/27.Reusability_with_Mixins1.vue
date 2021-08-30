<template>
  <div>
    <h2 @mouseover="incrementCount">Hovered {{ count }} times</h2>
  </div>
</template>

<script>

import CounterMixin from "../../27.mixins/counter";

//50.Reusability with Mixins -

export default {
  name: "HoverCounter",
  mixins: [CounterMixin],
//   data() {
//     return {
//       count: 0,
//     };
//   },
//   methods: {
//     incrementCount() {
//       this.count += 1;
//     },
//   },
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
