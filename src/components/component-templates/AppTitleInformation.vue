<template>
  <div class="app-title-information container">
    <div class="title app-title-information__title">
      Мы делаем регистрацию простой и понятной
    </div>
    <div class="text app-title-information__text">
      Получайте SMS-сообщения онлайн на виртуальный номер для регистрации в
      различных социальных сетях, интернет-магазинах и онлайн-сервисах абсолютно
      анонимно
    </div>
    <button :class="innerClass">Начать</button>
  </div>
</template>
<script>
export default {
  name: "AppTitleInformation",
  props: {
    hasLeft: Boolean,
    hasCenter: Boolean,
    hasAppTitleInfoButton: Boolean,
    hasButton: Boolean,
  },
  computed: {
    innerClass() {
      return {
        "--left": this.hasLeft,
        "--center": this.hasCenter,
        "app-title-information__button": this.hasAppTitleInfoButton,
        "button": this.hasButton,
      };
    },
  },
};
</script>
<style scoped>
.app-title-information {
  max-width: 700px;
  padding: 0 56px 37px 56px;
}

.app-title-information__text {
  margin-top: 62px;
}

.--center {
  margin-left: 210px;
}

.app-title-information__button {
  margin-top: 34px;
}
</style>