<template>
    <v-card
            class="mx-auto"
            max-width="400"
    >
        <v-img
                class="white--text align-end"
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
        >
            <v-card-title>Top 10 Australian beaches FUCK Nagasuck</v-card-title>
        </v-img>

        <v-card-subtitle class="pb-0">Number 10</v-card-subtitle>

        <v-card-text class="text--primary">
            <div>Whitehaven Beach</div>
            {{$auth.$state.loggedIn}}
        </v-card-text>


        <v-card-text class="text--primary">
            <div>Whitehaven Beach</div>
            {{fromLaravel}}
        </v-card-text>


        <v-card-actions>

            <v-btn
                    color="orange"
                    text
            >
                Share
            </v-btn>

            <v-btn
                    color="orange"
                    text
            >
                Explore
            </v-btn>
        </v-card-actions>
    </v-card>

</template>

<script>
    export default {
        data() {
            return {
                fromLaravel: ''
            }
        },
        mounted() {
            this.fromL()
        },
        methods: {
            async fromL() {
                let result = await this.$axios.get('test')
                this.fromLaravel = result.data.data
                console.log(result.data.data)
            }
        }
    }
</script>

<style>

</style>
