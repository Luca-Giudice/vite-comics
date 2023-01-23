<script>
export default {
    name: 'AppHeader'
}
</script>

<template>
<header>
    <div class="container">

        <figure>
            <a href="#"><img src="../src/assets/img/dc-logo.png" alt="dc comics"></a>
        </figure>
        <nav>
            <ul>
                <li><a href="#">CHARACTERS</a></li>
                <li><a href="#">COMICS</a></li>
                <li><a href="#">MOVIES</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">GAMES</a></li>
                <li><a href="#">COLLECTIBLES</a></li>
                <li><a href="#">VIDEOS</a></li>
                <li><a href="#">FANS</a></li>
                <li><a href="#">NEWS</a></li>
                <li><a href="#">SHOP</a></li>
                
            </ul>
        </nav>
    </div>
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
    padding: 4px;
    color: black;
    text-decoration: solid;
    font-size: 13px;
}

ul li a:hover {
   color: dodgerblue;
}



header .container{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 10px;
    gap: 40px;

}
</style>