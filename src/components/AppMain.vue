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
            ],
            products: [
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX',
                    price: '$19.99',
                    series: 'Action Comics',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01',
                    price: '$3.99',
                    series: 'American Vampire 1976',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb',
                    price: '$16.99',
                    series: 'Aquaman',
                    type: 'graphic novel',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76',
                    price: '$2.99',
                    series: 'Batgirl',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
                    price: '$3.99',
                    series: 'Batman',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ',
                    price: '$2.99',
                    series: 'Batman Beyond',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8',
                    price: '$3.99',
                    series: 'Batman/Superman',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk',
                    price: '$4.99',
                    series: 'Batman/Superman Annual',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8',
                    price: '$5.99',
                    series: 'Batman: The Joker War Zone',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY',
                    price: '$6.99',
                    series: 'Batman: Three Jokers',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX',
                    price: '$4.99',
                    series: 'Batman: White Knight Presents: Harley Quinn',
                    type: 'comic book',
                },
                {
                    thumb:
                        'https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq',
                    price: '$16.99',
                    series: 'Catwoman',
                    type: 'graphic novel',
                },
            ],

        }
    }
};
</script>


<template>
    <main>
        <section id="products">
            <div class="container card-container">
                <div v-for="product in products" :key="product.series" class="prod-card"><img :src="product.thumb" :alt="product.series"> <p>{{ product.series }}</p></div>
                
            </div>
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

.card-container{
    display: flex;
    flex-wrap: wrap;
    margin-top: 5rem 5rem ;
    .prod-card{
        width: 150px;
        height: 150px;
        gap: 10px;
        background-color: black;
        img{
            width: 90%;
            height: 90%;

        }
        a{
            color: white;
        }
    }
}
</style>