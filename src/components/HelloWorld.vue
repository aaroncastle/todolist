<template>
  <div class="hello">
    <h2> {{msg}} </h2>
    <h3> {{name}}</h3>
  </div>
</template>

<script>
const listObj = {
  name :  'solo'
};
export default {
  props: {
    msg: String
  },
  data() {
    return {
      name: listObj.name ? listObj.name : ''
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello {
  border : 0.1rem solid #2c3e50;
  height: 20rem;
}
</style>
