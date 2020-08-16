<template>
  <header>
    <nuxt-link to="/" class="logo"> Forum </nuxt-link>
    <nav>
      <ul>
          <li><nuxt-link to="/">Home</nuxt-link></li>
          <li><nuxt-link to="about">About</nuxt-link></li>
            <v-btn elevation="2"> Login </v-btn>
      </ul>
    </nav>
  </header>
</template>
<script>
export default {
}
</script>
<style>
  header {
      background: rgb(0, 000, 000);
      display: grid;
      grid-template-columns: repeat(2,auto);
  }
  .logo, li a {
      padding: 1em 2em;
      display: block;
      text-transform: uppercase;
      text-decoration: none;
      font-weight: bold;
      color: white;
      font-size: .9em;
  }
  nav {
      justify-self: right;
  }
  ul {
      list-style-type: none;
  }
  li {
      display: inline;
  }
  li a {
      padding: 1em 2em;
      display: inline-block;
      background: rgba(0,0,0,0.1);
  }
</style>