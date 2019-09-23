<template>
    <v-card>
        <v-card-title>
            <div>
                <h3> {{ person.name }} </h3>
                <div>
                    {{ person.gender }}
                </div>
                <span> {{ person.height }} </span>
            </div>
        </v-card-title>
        <v-card-actions>
            <v-btn>Choose</v-btn>
        </v-card-actions>
    </v-card>
</template>

<script>
export default {
    props: ["person"],
    filters: {
        allCaps(value) {
            return value.toUpperCase()
        }
    }
}
</script>

<style scoped>

</style>