<template>
  <div>
    <PopupCard v-if="cardData !== null" v-bind:cardData="cardData" />

    <TopicCard v-for="topic in topics" v-bind:topic="topic"/>      
  </div>
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
      topics: [{
        id: 1,
        title: "Socialism",
        desc: "What is it and how does it affect?",
      }, {
        id: 2,
        title: "Capitalism",
        desc: "What is it and how does it affect?"
      }, {
        id: 3,
        title: "Market",
        desc: "What is the purpose of a market and how does it work?"
      }]
    };
  },
  // data() {
  //   return {
  //     topics: [{
  //       id: 1,
  //       title: "Socialism",
  //       desc: "What is it and how does it affect?",
  //     }, {
  //       id: 2,
  //       title: "Capitalism",
  //       desc: "What is it and how does it affect?"
  //     }, {
  //       id: 3,
  //       title: "Market",
  //       desc: "What is the purpose of a market and how does it work?"
  //     }],  
  //   }
  // },
  async fetch() {
    // this.mountains = await fetch(
    //   "https://api.nuxtjs.dev/mountains"
    // ).then((res) => res.json());
  },
};
</script>

<style>
</style>