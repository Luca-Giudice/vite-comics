<script>
export default {
    name: 'AppMain'
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
                    <li>
                        <a href="#"><img src="../assets/img/buy-comics-digital-comics.png" alt=""> <p>DIGITAL COMICS</p></a>
                        
                    </li>
                    <li>
                        <a href="#"><img src="../assets/img/buy-comics-merchandise.png" alt=""> <p>DIGITAL COMICS</p></a>
                    </li>
                    <li>
                        <a href="#"><img src="../assets/img/buy-comics-shop-locator.png" alt=""> <p>DIGITAL COMICS</p></a>
                    </li>
                    <li>
                        <a href="#"><img src="../assets/img/buy-comics-subscriptions.png" alt=""> <p>DIGITAL COMICS</p></a>
                    </li>
                    <li>
                        <a href="#"><img src="../assets/img/buy-dc-power-visa.svg" alt="">
                            <p>DC POWER VISA</p>
                        </a>
                    </li>
                    
                </ul>
            </div>

        </section>
    </main>
</template>

<style scoped>
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
}
#merch ul{
    display: flex;
    justify-content: center;
    gap: 5px;
}

ul li{
    list-style-type: none;
}
#merch a{
    display: flex;
    align-items: center;

    gap: 10px;
}

#merch img{
    width: 20%;
}
h2{
    color: white;
}


a{
    color: wheat;
}
</style>