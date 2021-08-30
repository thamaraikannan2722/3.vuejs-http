<template>
  <div>
    Parent Component
    <button @click="showChild = !showChild">Toggle Child</button>
    <Child v-if="showChild" />
  </div>
</template>

<script>
//46.Component Lifecycle Hooks - Creation, Mounting, Updating, Unmounting, MISC.
//1.Creation - beforeCreate(), created().
//2.Mounting - beforeMount(), Mounted().
//3.Updating - beforeUpdate(), Updated().
//4.Unmounting - beforeUnmount(), Unmounted().
//5.MISC -activated(), deactivated(), errorCaptured, renderTracked(), renderTriggered.

import Child from "../25.Component Lifecycle Hooks/Child";

export default {
  name: "Parent",
  components: { Child },
  data() {
    return {
        showChild: true,
    };
  },
  beforeCreate() {
    console.log('Parent beforeCreate()')
  },
  created() {
    console.log('Parent created()')
  },
  beforeMount() {
    console.log('Parent beforeMount()')
  },
  mounted() {
    console.log('Parent mounted()')
  },
  beforeUpdate() {
    console.log('Parent beforeUpdate()')
  },
  updated() {
    console.log('Parent updated()')
  },
  beforeUnmount() {
    console.log('Parent beforeUnmount()')
  },
  unmounted() {
    console.log('Parent unmounted()')
  },
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
