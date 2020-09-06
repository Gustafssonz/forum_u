<template>
      <v-card>
          <v-card-title> {{ topic.title }} </v-card-title>
          <v-card-text> {{ topic.desc }} </v-card-text>
            <nuxt-child to="/1">
              next
              </nuxt-child>

      </v-card>
</template>

<script>
    export default {
    data() {
      return {
        // topic: []
      }
    },
    props: ['topic'],
    methods: {
      openCard(){

      }
    }

  }
</script>

<style lang="scss" scoped>

</style>