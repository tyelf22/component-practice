<template>
    <v-card>
        <v-card-title>{{ name }}</v-card-title>
        <v-card-text>My custom component</v-card-text>
    </v-card>
</template>

<script>
export default {
   data: () => {
       return {
           name: 'Tyson Elfors'
       }
   } 
}
</script>

<style>

</style>