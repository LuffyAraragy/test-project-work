<template>
  <div class="app-component container">
    <div class="title app-component__title">Как это работает?</div>
    <div class="app-component__block-all">
      <div :class="innerClass">
        <img src="@/assets/icon/Id.png" alt="" class="app-component__icon" />
        <div class="app-component__block-text">
          <div class="title app-component__title">Получение номера</div>
          <div class="text app-component__text">
            Получите виртуальный номер в личном кабинете, скопируйте и вставьте
            его в нужный сервис для получения SMS-сообщения.
          </div>
        </div>
      </div>

      <div :class="innerClass">
        <img src="@/assets/icon/Id.png" alt="" class="app-component__icon" />
        <div class="app-component__block-text">
          <div class="title app-component__title">Получение номера</div>
          <div class="text app-component__text">
            Получите виртуальный номер в личном кабинете, скопируйте и вставьте
            его в нужный сервис для получения SMS-сообщения.
          </div>
        </div>
      </div>

      <div :class="innerClass">
        <img src="@/assets/icon/Id.png" alt="" class="app-component__icon" />
        <div class="app-component__block-text">
          <div class="title app-component__title">Получение номера</div>
          <div class="text app-component__text">
            Получите виртуальный номер в личном кабинете, скопируйте и вставьте
            его в нужный сервис для получения SMS-сообщения.
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppComponent",
  props: {
    hasRow: Boolean,
    hasColumn: Boolean,
  },
  computed: {
    innerClass() {
      return {
        "--row": this.hasRow,
        "--column": this.hasColumn,
      };
    },
  },
};
</script>

<style scoped>
.app-component {
  text-align: center;
}

.app-component__block-all {
  display: flex;
  gap: 20px;
}

.--row {
  margin-top: 120px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.--column {
  margin-top: 120px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.app-component__icon {
  max-width: 130px;
  max-height: 140px;
}

.app-component__block-text {
  margin-top: 47px;
  display: flex;
  gap: 47px;
  flex-direction: column;
}
</style>