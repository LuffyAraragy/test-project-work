<template>
  <div class="page-home">
    <AppHeader> </AppHeader>
    <AppTitleInformation :hasButton="true" :hasLeft="true" :hasAppTitleInfoButton="true"> </AppTitleInformation>
    <AppComponent :hasColumn="true"> </AppComponent>
    <AppComponent :hasRow="true"> </AppComponent>
    <AppContentBankCard> </AppContentBankCard>
    <AppFormMessage> </AppFormMessage>
    <AppFooter> </AppFooter>
  </div>
</template>

<script>
import AppHeader from "@/components/AppHeader.vue";
import AppFooter from "@/components/AppFooter.vue";
import AppTitleInformation from "@/components/component-templates/AppTitleInformation.vue";
import AppComponent from '@/components/component-templates/AppComponent.vue';
import AppContentBankCard from '@/components/AppContentBankCard.vue';
import AppFormMessage from '@/components/AppFormMessage.vue';

export default {
  components: { AppHeader, AppFooter, AppTitleInformation, AppComponent, AppContentBankCard, AppFormMessage },
  name: "PageHome",
};
</script>

<style scoped>
</style>