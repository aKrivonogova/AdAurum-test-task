<template>
        <button :class="['header__button', modifier]"></button>
</template>
<script>
export default {
    name: 'header-button-component',
    props:{
        modifier: String,
    },
};
</script>
<style lang="scss">
.header{
    &__button{
        width: $circleButtonWidth;
        height: $circleButtonHeight;
        border: none;
        outline: none;
        background-color: $background-theme-light;
        border-radius: $circleButtonBorderRadius;
        background-position: center;
        background-repeat: no-repeat;
        background-size: $primaryButtonLogoWidth $primaryButtonLogoHeight;

        &--settings{
            margin-right: 12px;
            background-image: url('../../assets/images/settings.svg');
        }

        &--logout{
            background-image: url('../../assets/images/login.svg');
        }
    }
}
</style>