<template>
  
<PostList />
<CreatePost />
<Parent />
<TemplateRefs />
<ClickCounter />
<HoverCounter />

</template>

<script>

import PostList from "../src/components/23.HTTP_GET_Request";
import CreatePost from "../src/components/24.HTTP_POST_Request";
import Parent from "../25.Component Lifecycle Hooks/Parent";
import TemplateRefs from "../src/components/26.TemplateRefs";
import ClickCounter from "../src/components/27.Reusability_with_Mixins";
import HoverCounter from "../src/components/27.Reusability_with_Mixins1";

export default {
  name: 'App',
  components: {
    PostList,
    CreatePost,
    Parent,
    TemplateRefs,
    ClickCounter,
    HoverCounter,
  },
}
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
