<template>
<p class="header__text">
    <slot></slot>
</p>
</template>

<script>
export default {
    name: 'header-text-component',
}
</script>

<style lang="scss">
.header {
    &__text{
        font-weight: $fontWeightSemibold;
        margin-right: 26px;
        font-size: $fontSazeMedium;
        color: $primaryColor;
    }
}
</style>
