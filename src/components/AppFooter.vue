<script>
import AppFooterTop from './AppFooterTop.vue';
import AppFooterCenter from './AppFooterCenter.vue';
import AppFooterBottom from './AppFooterBottom.vue';

export default {
    data() {
        return {

        }
    },
    components: {
        AppFooterTop,
        AppFooterCenter,
        AppFooterBottom,
    }
}
</script>

<template>
    <AppFooterTop></AppFooterTop>
    <AppFooterCenter></AppFooterCenter>
    <AppFooterBottom></AppFooterBottom>
</template>

<style lang="scss" scoped></style>