<template>
    <div class="header__info-block">
        <slot></slot>
    </div>
</template>
<script>
export default {
    name: 'header-info-block-component',
};

</script>
<style lang="scss">
.header__info-block{
    display: flex;
    align-items: center;
}
</style>