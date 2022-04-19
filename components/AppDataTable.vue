<template>
    <v-row justify="center" align="center">
        <v-col>
        <v-card class="py-4 d-flex justify-center">
            <template>
            <v-data-table
                :headers="header"
                :items="data"
                :items-per-page="10"
                class="elevation-1"
            ></v-data-table>
            </template>
        </v-card>
        </v-col>
    </v-row>
</template>

<script>
    export default {
        name: 'AppDataTable',
        props: ['header','data']
    }
</script>

<style lang="scss" scoped>

</style>