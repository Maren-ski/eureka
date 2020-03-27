<template>
  <div id="app">
    <Header/>
    <UserList v-bind:users= "users"/>

  </div>
</template>

<script>
import UserList from './components/UserList.vue'
import Header from './components/Header.vue'

export default {
  name: 'App',
  components: {
    UserList,
    Header
  },
  data() {
    return {
      users: [
        {userId: "1", userName: "John", feesPaid: false},
        {userId: "2", userName: "Mary", feesPaid: true},
        {userId: "3", userName: "Salma", feesPaid: false}
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
