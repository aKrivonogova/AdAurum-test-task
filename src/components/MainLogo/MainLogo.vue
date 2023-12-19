<template>
<img :src="imageSrc" alt="логотип сайта" :class="['main-logo',modifer]">
</template>

<script>
export default {
    name: 'main-logo-component',
    props: {
        modifer: String,
        imageSrc: String
    }
}
</script>

<style lang="scss">
.main-logo {
    width: $primaryImageWidth;
    height: $primatyImageHeight;
    &--top{
        margin-top: 3px;
    }
}
</style>
