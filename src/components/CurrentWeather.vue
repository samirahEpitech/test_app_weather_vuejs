<template>
<div class="hello">
    <weather
        api-key="<your-dark-sky-api-key>"
        title="Weather"
        latitude="24.886436"
        longitude="91.880722"
        language="en"
        units="uk">
    </weather>
  <div>
    <select v-model="selected">
      <option disabled value="">Choisissez</option>
      <option >Paris</option>
      <option >Lyon</option>
      <option >Marseille</option>
      <option >Toulouse</option>
      <option >Strasbourg</option>
    </select>
    <span>Selectionné : {{ selected }}</span>
  </div>
</div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
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
