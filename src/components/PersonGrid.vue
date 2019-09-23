<template>
    <v-container>
        <v-row>
            <v-col cols="3" v-for="person in people" :key="person.name">
                <star-wars-person :person="person"></star-wars-person>
            </v-col>
        </v-row>
    </v-container>

</template>

<script>

import StarWarsPerson from "../components/StarWarsPerson"


export default {
    props: ["people"],
    components: {
        StarWarsPerson
    }
}
</script>

<style scoped>

</style>