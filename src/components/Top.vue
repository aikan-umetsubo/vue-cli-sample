<template>
  <div class="top">
    <h1>Vue CLIを使って作ってみたSPA</h1>
    <h3>Cat Fact</h3>
    <p>
      axiosを使って<a href="https://alexwohlbruck.github.io/cat-facts/">cat-facts</a>から取得した猫の話を表示します
    </p>
    <blockquote id="cat-fact">
      {{ cat_fact }}
    </blockquote>
  </div>
</template>

<script>
import axios from 'axios'

export default {
  name: 'Top',
  data: () => {
    return {
      cat_fact: 'loading'
    }
  },
  mounted: function(){
    axios
      .get('https://cat-fact.herokuapp.com/facts/random')
      .then(response => {
        console.log(response);
        this.cat_fact = response.data.text
      })
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
#cat-fact {
  padding: 1em;
  width: 40em;

  position: relative;
  left: calc(50% - 23em);
  background-color: darkgray;
}
a {
  color: #42b983;
}
</style>
