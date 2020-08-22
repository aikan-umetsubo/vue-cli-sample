<template>
  <div class="home">
    <Top msg="This is the top page"/>
  </div>
</template>

<script>
// @ is an alias to /src
import Top from '@/components/Top.vue'

export default {
  name: 'Home',
  components: {
    Top
  }
}
</script>
