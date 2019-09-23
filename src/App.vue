<template>
  <v-app>
    <projHeader/>
    <hr>
    <v-container align-center>
      <v-row>
        <server/>
        <serverDetails/>
      </v-row>
    </v-container>
    <hr>
    <projFooter/>
  </v-app>
</template>

<script>
import projHeader from './components/Header'
import server from './components/Server'
import serverDetails from './components/ServerDetails'
import projFooter from './components/projFooter'

export default {
  name: 'App',
  components: {
    projHeader,
    server,
    serverDetails,
    projFooter
  },
  props: {
    currentServer: {
      default: 0,
      type: Number
    },
    currentServerStatus: {
      default: 'Server Details are currently unavailable',
      type: String
    }
  },
  data: () => {
    return {
      //
    }
  },
  
}
</script>
