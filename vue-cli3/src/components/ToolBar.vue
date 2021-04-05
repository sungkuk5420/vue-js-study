<template>
<div>
    <router-link to="News">News</router-link>
    <router-link to="Ask">Ask</router-link>
    <router-link to="Jobs">Jobs</router-link>
</div>
</template>

<script>
export default {
  name: 'ToolBar',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
