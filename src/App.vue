<template>
  <div class="app" id="app">
    <PageHome/>
  </div>
</template>

<script>
import PageHome from './pages/PageHome.vue';

export default {
  name: 'App',
  components: {
    PageHome,
  }
}
</script>

<style>
* {
  margin: 0;
  padding: 0;
}

.container {
  margin: 0 auto;
  max-width: 1160px;
  padding: 0 20px;
}

</style>
