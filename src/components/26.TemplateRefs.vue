<template>
  <div>
    <input type="text" ref="inputRef" />
    <PostList ref="postListRef" />
  </div>
</template>

<script>
import PostList from "../../src/components/23.HTTP_GET_Request";

//49.Template Refs -

export default {
  name: "TemplateRefs",
  components: {
    PostList,
  },
  data() {
    return {};
  },
  mounted() {
    console.log(this.$refs.postListRef);
    this.$refs.inputRef.focus();
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
