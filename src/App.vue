<script>
import AppHeader from './AppHeader.vue';
export default {
    name: 'comics',
    components: {AppHeader}
}
</script>


<template>
    <app-header></app-header>
    <main></main>
    <footer></footer>
</template>

<style>
/* reset */
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
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