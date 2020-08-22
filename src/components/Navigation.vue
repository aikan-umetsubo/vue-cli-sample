<template>
  <div id="nav">
    <div id="title">
      <span>Vue CLI 試しに作ってみたページ</span>
    </div>
    <div id="pages">
      <ul>
        <li><router-link to="/">Home</router-link></li>
        <li><router-link to="/about">About</router-link></li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Navigation',
  props: {
  }
}
</script>

<style scoped>
#nav {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
}

#title span {
  text-align: left;
  top: calc(50% - 1eh);
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
