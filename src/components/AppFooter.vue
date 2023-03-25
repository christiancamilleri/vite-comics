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
    <footer>

        <AppFooterTop></AppFooterTop>
        <AppFooterCenter></AppFooterCenter>
        <AppFooterBottom></AppFooterBottom>

    </footer>
</template>

<style lang="scss" scoped></style>