<template>

  <PopupCard 
  v-if="cardData !== null" 
  v-bind:cardData="cardData" 
  />

</template>

<script>

export default {
  data: function () {
    return {
      cardData: {
        title: "First time visiting Forum?",
        text: "Here you get an overview of all the things going on, click here to get a guided tour!",
        buttonText: "Another time",
        special: true
      },
    }
  },
}
</script>
<style>
</style>