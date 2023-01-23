<script>
export default {
    name: 'AppHeader'
}
</script>

<template>
<header>
    <figure>
        <a href="#"><img src="../src/assets/img/dc-logo.png" alt="dc comics"></a>
    </figure>
    <nav>
        <ul>
            <li><a href="">capitalize</a></li>
        </ul>
    </nav>
</header>
</template>

<style scoped>
figure {
    text-align: center;
}

ul{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 30px;
    padding: 0;
}

ul li{
    list-style-type: none;

}

ul li a {
    padding: 10px;
}
    
</style>