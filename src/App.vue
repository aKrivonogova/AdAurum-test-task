<template>
<HaderComponent>
</HaderComponent>
<MainComponent></MainComponent>
<FooterComponent></FooterComponent>
</template>

<script>
import HaderComponent from './components/Header/Header.vue';
import FooterComponent from './components/Footer/Footer.vue';
import MainComponent from './components/Main/Main.vue'
export default {
    name: 'App',
    components: {
        HaderComponent,
        FooterComponent,
        MainComponent
    }
}
</script>

<style lang="scss">
@import '../fonts/fonts.css';
* {
    margin: 0;
    padding: 0;
}

;

#app {
    background-color: $mainBackground;
    font-family: 'Inter'
};
</style>
