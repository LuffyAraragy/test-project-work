<template>
  <div class="app-form-message container">
    <div class="title app-form-message__title">Написать нам</div>
    <div class="app-form-message__message">
      <input type="text" />
      <input type="text" />
      <input type="text" />
      <div class="app-form-message__block-checkbox">
        <input type="checkbox" />
        <div class="text app-form-message__text">
          Я соглашаюсь с политикой конфиденциальности и использованием
          запрашиваемых данных
        </div>
      </div>
      <button class="button button app-form-message__button">Отправить</button>
    </div>
  </div>
</template>
<script>
export default {
  name: "AppFormMessage",
};
</script>
<style scoped>
.app-form-message {
  display: flex;
}

.app-form-message__title {
  margin-top: 235px;
}

.app-form-message__message {
  max-width: 500px;
  padding: 32px;
  display: grid;
  justify-content: center;
  gap: 26px;
}

.app-form-message__block-checkbox {
  display: flex;
  gap: 13px;
}

.app-form-message__button {
  margin: 0 auto;
  max-width: 200px;
}
</style>