<template>
  <div class="hello">
     Token: {{token}}
  </div>
</template>

<script>
import { reactive } from '@vue/reactivity'
export default {
  name: 'HelloWorld',
  data(){
    return{
      token: reactive(sessionStorage.getItem('token'))
    }  
  },
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
