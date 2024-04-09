<template>
  <div class="app" id="app">
    <PageHome />
  </div>
</template>

<script>
import PageHome from "./pages/PageHome.vue";

export default {
  name: "App",
  components: {
    PageHome,
  },
};
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

.title {
  font-size: 44px;
  font-weight: 700;
  line-height: 60px;
}

.text {
  font-size: 20px;
  font-weight: 400;
  line-height: 34px;
}

.button {
  padding: 5px 20px;
  font-size: 20px;
  font-weight: 500;
  border-radius: 14px;
  color: #ffffff;
  background-color: #1890ffa1;
  border: none;
}

.button-header {
  padding: 8px 13px;
  font-size: 13px;
  font-weight: 500;
  border-radius: 30px;
  color: #ffffff;
  background-color: #1890ffa1;
  border: none;
}
</style>
