<template>
  <div id="app">
  <ul>
    <li>
      <p>{{ moment(date).format('MMMM Do YYYY, h:mm:ss a') }}</p>
      <currentWeather currentDate="11 Septembre 2019"/>
    </li>
  </ul>
</div>
</template>
<script>
import currentWeather from './components/CurrentWeather.vue'
export default {
  name: 'App',
  components: {
    currentWeather
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
