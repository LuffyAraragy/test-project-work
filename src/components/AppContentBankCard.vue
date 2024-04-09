<template>
    <div class="app-content-bank-card container">
        <img src="@/assets/img/Group 14.png" alt="" class="app-content-bank-card__img">
        
        <AppTitleInformation :hasButton="true" :hasCenter="true" :hasAppTitleInfoButton="true">

        </AppTitleInformation>
    </div>
</template>
<script>
import AppTitleInformation from './component-templates/AppTitleInformation.vue';

export default {
    name: "AppContentBankCard",
    components: {
        AppTitleInformation,
    }
}
</script>
<style scoped>
.app-content-bank-card {
    margin-top: 160px;
    display: flex;
    align-items: center;
}

.app-content-bank-card__img {
    width: 100%;
    max-width: 450px;
    min-width: 200px;
}
</style>