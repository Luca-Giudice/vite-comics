<script>
export default {
    name: 'AppMain',
    data(){
        return{
            images:[
                { img:'../assets/img/buy-comics-digital-comics.png', text:'DIGITAL COMICS'},
                { img: '../assets/img/buy-comics-merchandise.png', text: 'DC MERCHANDISE' },
                { img: '../assets/img/buy-comics-shop-locator.png', text: 'SUBSCRITION' },
                { img: '../assets/img/buy-comics-subscriptions.png', text: 'COMIC SHOP LOCATOR' },
                { img: '../assets/img/buy-dc-power-visa.svg.png', text: 'DC POWER VISA' },
            ]
        }
    }
};
</script>


<template>
    <main>
        <section id="products">
            <h2>content goes heare</h2>
        </section >
        <section id='merch'>
            <div class="container">

                <ul>
                    <li v-for="image in images" :key="image.img">
                        <a href="#"><img :src="image.img" alt="#"> <p>{{image.text}}</p></a>
                        
                    </li>
                   
                    
                </ul>
            </div>

        </section>
    </main>
</template>

<style lang="scss" scoped>
#products{
    background-color: black;
    text-align: center;
    margin-top: 1rem;
    padding: 4rem 1rem;
}
#merch{
    background-color: rgb(2, 130, 249);
    text-align: center;
    padding: 3rem 3rem;
    ul{
        display: flex;
        justify-content: center;
        gap: 5px;
        
        li{
            list-style-type: none;
        }
    }
    a{
        display: flex;
        align-items: center;
        
        gap: 10px;
    }
    img{
        width: 20%;
    }
}
h2{
    color: white;
}


a{
    color: wheat;
}
</style>