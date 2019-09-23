<template>
  <v-app>
    <v-content>
      <person-grid :people="people"></person-grid>
     <!--  <v-btn @click="getData">Get Data!!</v-btn> -->
    </v-content>
  </v-app>
</template>

<script>
import PersonGrid from './components/PersonGrid'
//import { people } from './assets/people'
import axios from 'axios'

export default {
  name: 'App',
  components: {
    PersonGrid,
  },
  data: () => {
    return {
      people: [],
    }
  },
  created: function () {
    // `this` points to the vm instance
    let vm = this
      return axios.get('https://swapi.co/api/people').then(response => {
        vm.people = response.data.results
      }).catch(error => console.error(error))
  },
  methods: {
    getData() {
      let vm = this
      return axios.get('https://swapi.co/api/people').then(response => {
        vm.people = response.data.results
      }).catch(error => console.error(error))
    }
  }
}
</script>
