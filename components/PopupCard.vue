<template>
    <v-col v-if="show" cols="6">
        <v-card 
        class="mx-auto" 
        color="success" 
        >
            <v-card-title class="headline">{{ cardData.title }}</v-card-title>
            <v-card-subtitle>{{ cardData.text }}</v-card-subtitle>
            <v-card-actions>
            <v-btn @click="removeMessage(1)" text> {{ cardData.buttonText }}</v-btn>
            </v-card-actions>
        </v-card>
    </v-col>
</template>
<script>  
  export default {
        data() {
            return { show : true }
        },
        props: ['cardData'],
        methods: {
             removeMessage(seconds) {
                this.show = false;
            },
        }
  }
</script>

<style>
</style>
