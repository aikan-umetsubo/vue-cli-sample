<template>
  <div id="nav">
    <div>
      <div>
        Vue CLI 試しに作ってみたページ
      </div>
    </div>
    <div>
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
div#nav {
  display: flex;
  flex-direction: row;
}

div#nav div {
  flex: 1 0 fit-content;
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
