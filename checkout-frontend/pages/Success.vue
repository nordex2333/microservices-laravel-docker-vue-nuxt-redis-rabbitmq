<template>
  <div class="container">
    <div class="py-5 text-center">
      <h2>Success</h2>
      <p class="lead">Your purchase has been completed!</p>
    </div>
  </div>
</template>

<script>
import Vue from 'vue'
import axios from '../plugins/axios';

export default Vue.extend({
  async mounted() {
    const {data} = await axios.post('/orders/confirm', {
      source: this.$route.query.source
    });

    console.log(data);
  }
})
</script>
