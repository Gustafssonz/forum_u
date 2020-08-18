<template>
  <PopupCard v-if="cardData !== null" 
  v-bind:cardData="cardData"
  />
</template>

<script>
export default {
  asyncData(context) {
    return {
      cardData: {
        title: "First time at Topics?",
        text: "Here you can check out all the cool topics on the forum",
        buttonText: "Press here to remove the card",
      },
    };
  },
};
</script>

<style>
</style>