<script>
import AppMain from './components/AppMain.vue';
import AppHeader from './AppHeader.vue';
import AppFooter from './components/AppFooter.vue';

export default {
    name: 'comics',
    components: {AppHeader, AppMain, AppFooter},
}
</script>


<template>
    <app-header></app-header>
    <app-main></app-main>
    <app-footer></app-footer>
</template>

<style>
/* reset */
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* stile */
*{
    font-family: sans-serif;
}

img{
    max-width: 100%;
    height: auto;
}

a {
    text-decoration: none;
}

.container{
    margin: 0 auto;
    max-width: 1140px;
}
</style>