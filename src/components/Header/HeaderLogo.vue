<template>
<div :class="['header__logo', modifer]">
    <img :src="imageSrc" alt="Картинка" class="header__logo-source">
</div>
</template>

<script>
export default {
    name: 'header-logo-component',
    props: {
        modifer: String,
        imageSrc: String
    }
}
</script>

<style lang="scss">
.header {
    &__logo {
        width: $circleButtonWidth;
        height: $circleButtonHeight;
        border-radius: $circleButtonBorderRadius;
        background-color: $primaryButtonBackground;
        display: flex;
        align-items: center;
        justify-content: center;

        &--progress {
            margin-right: 8px;
        }

        &--user {
            margin-right: 10px;
        }
    }

    &__logo-source {
        width: $primaryButtonLogoWidth;
        height: $primaryButtonLogoHeight;
    }
}
</style>
