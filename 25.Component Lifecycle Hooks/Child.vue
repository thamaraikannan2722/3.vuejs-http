<template>
  <div>Child Component</div>
</template>

<script>

//46.Component Lifecycle Hooks - Creation, Mounting, Updating, Unmounting, MISC.
//1.Creation - beforeCreate(), created(). 
//2.Mounting - beforeMount(), Mounted().
//3.Updating - beforeUpdate(), Updated().
//4.Unmounting - beforeUnmount(), Unmounted().
//5.MISC -activated(), deactivated(), errorCaptured, renderTracked(), renderTriggered.

export default {
  name: "Child",
  beforeCreate() {
    console.log('Child beforeCreate()')
  },
  created() {
    console.log('Child created()')
  },
  beforeMount() {
    console.log('Child beforeMount()')
  },
  mounted() {
    console.log('Child mounted()')
  },
  beforeUpdate() {
    console.log('Child beforeUpdate()')
  },
  updated() {
    console.log('Child updated()')
  },
  beforeUnmount() {
    console.log('Child beforeUnmount()')
  },
  unmounted() {
    console.log('Child unmounted()')
  },
  data() {
    return {
    };
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