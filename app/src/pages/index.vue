<template>
  <v-row justify="center" align="center">
    Index Page
  </v-row>
</template>

<script>
export default {
  name: 'IndexPage',
  created() {
    this.testApi();
  },
  methods: {
    testApi() {
      this.$api.get('/test').then(response => {
        console.log(response);
      })
    }
  }
}
</script>
