<template>
<header class="header">
    <div class="header__container">
        <MainLogo :modifer="mainLogoModifer.mainLogoTopModifer" :imageSrc="imagesList.mainLogo"></MainLogo>
        <div class="header__content">
            <HeaderInfoBlock>
                <HeaderLogo :modifer="headerModiferesList.headerProgressModiger" :imageSrc="imagesList.convertCard"></HeaderLogo>
                <HeaderText>5%</HeaderText>
            </HeaderInfoBlock>
            <HeaderInfoBlock>
                <HeaderLogo :modifer="headerModiferesList.headerLogoUserModifer" :imageSrc="imagesList.userLogo"></HeaderLogo>
                <HeaderText>Username@adaurum.ru
                </HeaderText>
            </HeaderInfoBlock>
            <HeaderButton :modifier="headerModiferesList.settingsButtonModifer"></HeaderButton>
            <HeaderButton :modifier="headerModiferesList.logoutButtonModifer"></HeaderButton>
        </div>
    </div>
</header>
</template>

<script>
import HeaderInfoBlock from './HeaderInfoBlock.vue';
import HeaderButton from './HeaderButton.vue';
import HeaderLogo from './HeaderLogo.vue';
import HeaderText from './HeaderText.vue';
import MainLogo from '@/components/MainLogo/MainLogo';
import headerModiferes from '../../../data/headerModiferes.json';
import mainLogoModiferes from '../../../data/mainLogo.json';
import imagesForPage from '../../../data/images'
export default {
    name: 'header-component',
    components: {
        HeaderInfoBlock,
        HeaderButton,
        HeaderLogo,
        HeaderText,
        MainLogo
    },
    data() {
        return {
            headerModiferesList: headerModiferes,
            mainLogoModifer: mainLogoModiferes,
            imagesList: imagesForPage,
        };
    },
}
</script>

<style lang="scss">
.header {
    width: 100%;
    background-color: transparent;
    padding-top: 33px;
    padding-bottom: 34px;
    &__container{
        display: flex;
        max-width: $primaryWidth;
        justify-content: space-between;
        margin-left: auto;
        margin-right: auto;
    }
    &__content{
        display: flex;
    }
    
}
</style>
