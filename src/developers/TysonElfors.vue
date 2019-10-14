<template>
    <v-card>
        <v-card-title>{{ name }}</v-card-title>
        <v-card-text>My custom component</v-card-text>
        <v-text-field counter="25" maxlength="25" label="input"></v-text-field>
    </v-card>
</template>

<script>
export default {
   data: () => {
       return {
           name: 'Tyson Elfors',
          
       }
   } 
}
</script>

<style>

</style>