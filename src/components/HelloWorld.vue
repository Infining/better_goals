<template>
  <div class="">
    <p>This is the message: {{ msg }}</p>
    <input type="button" @click="newMsg()" value="Update Message" />
    <p>This is my name: {{ gaulsName }}</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  },
  methods: {
    newMsg () {
      this.msg = 'New message'
    }
  },
  computed: {
    gaulsName () {
      return 'Nathan Gaul'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
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
