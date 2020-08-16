<template>
    <v-col cols="6">
        <v-card class="mx-auto" color="grey" dark>
        <v-card-title class="headline">{{ items.title }}</v-card-title>

        <v-card-subtitle>{{ items.text }}</v-card-subtitle>

        <v-card-actions>
        <v-btn text> {{ items.buttonText }}</v-btn>
        </v-card-actions>
        </v-card>
    </v-col>
</template>
<script>
  export default {
    data: () => ({
      items: {
        color: '##40414f',
        title: 'Welcome to FORUM',
        text: "Let's get you up to speed with that you can do",
        buttonText: "Let's get started!"
      }
    }),
  }
</script>

<style>
</style>
