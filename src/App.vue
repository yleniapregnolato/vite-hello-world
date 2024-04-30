<script>
import AppTitle from './AppTitle.vue';
import AppBanner from './components/AppBanner.vue';

export default {
    data() {
        return {};
    },
    components: { AppTitle, AppBanner }
}
</script>

<template>
  <section>
    <AppTitle />
    <AppBanner />
  </section>
</template>

<style></style>