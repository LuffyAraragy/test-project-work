<template>
  <div class="app-footer">
    <div class="app-footer__block-links">
      <img src="@/assets/icon/Logo set.png" alt="" />
      <div class="app-footer__social-network"></div>
      <div class="app-footer__social-network"></div>
    </div>
    <div class="app-footer__year">© 2020 Linearity Gmb</div>
    <div class="app-footer__text">
      Политика обработки персональных файлов и cookie
    </div>
  </div>
</template>
<script>
export default {
  name: "AppFooter",
};
</script>
<style scoped>
.app-footer {
    display: flex;
    justify-content: space-around;
    align-items: center;
}
.app-footer__block-links {
  display: flex;
  gap: 60px;
}
</style>