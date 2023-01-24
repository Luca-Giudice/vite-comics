<script>
export default {
    name: 'AppHeader',
    data(){
        return{
            links: [
                
                { text: 'CHARACTERS', ulr: '#'},
                { text: 'COMICS', ulr: '#'},
                { text: 'MOVIES', ulr: '#'},
                { text: 'TV', ulr: '#'},
                { text: 'GAMES', ulr: '#'},
                { text: 'COLLECTIBLES', ulr: '#'},
                { text: 'VIDEOS', ulr: '#'},
                { text: 'FANS', ulr: '#'},
                { text: 'NEWS', ulr: '#' },
                { text: 'SHOP', ulr: '#' }
            ]
        }
    }
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
                <li v-for="link in links" :key="link.text"><a :href="link.url" v-text="link.text"></a></li>
                
            </ul>
        </nav>
    </div>
</header>
</template>

<style lang="scss" scoped>
figure {
    text-align: center;
}

ul{
    display: flex;
    justify-content: center;
    align-items: center;
    margin: 30px;
    padding: 0;
    
    
    li{
        list-style-type: none;
        
        
        a {
            padding: 4px;
            color: black;
            text-decoration: solid;
            font-size: 13px;
        }
    }
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