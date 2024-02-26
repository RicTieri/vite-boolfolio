<script>
import axios from 'axios';
export default {
  name: 'AppMain',
  data() {

  },
  methods: {
    getProject() {
      axios.get('http://127.0.0.1:8000/api/projects', {
        params: {

        }
      })
        .then(function (response) {
          // handle success
          console.log(response.data);
        })
        .catch(function (error) {
          // handle error
          console.log(error);
        });
    }
  },
  created() {
    this.getProject()
  },
}
</script>

<template>
  <main>
    main
  </main>
</template>

<style lang="scss" scoped></style>