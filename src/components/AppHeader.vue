<template>
  <div class="app-header">
    <div class="app-header__icon">
        <img src="@/assets/icon/Logo set.png" alt="">
    </div>
    <div class="app-header__pages">
        <a href="" class="app-header__page">Получить смс</a>
        <a href="" class="app-header__page">Заработать</a>
        <a href="" class="app-header__page">Документация</a>
        <a href="" class="app-header__page">Блог</a>
    </div>
    <div class="app-header__block-button">
        <button class="button-header">
            RU V
        </button>
        <button class="button-header">
            Войти >
        </button>
    </div>
  </div>
</template>
<script>
export default {
  name: "AppHeader",
};
</script>
<style scoped>

.app-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.app-header__pages {
    display: flex;
    gap: 50px;
}

.app-header__block-button {
    display: flex;
    gap: 17px;
}
</style>