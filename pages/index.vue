<template>

  <Welcome v-if="firstTimer" />

</template>

<script>
import Welcome from '../components/Welcome';

export default {
  data () {
    return {
      firstTimer: true,
    }
  },
}
</script>
<style>
</style>