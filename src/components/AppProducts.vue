<script>

export default {

    name: 'AppProducts',

    data() {
        return{

            products: [
                {
                    img: 'product-item1.png',
                    avg: 5,
                    name: 'Cool-duck',
                    price: 15,
                },
                {
                    img: 'product-item2.png',
                    avg: 5,
                    name: 'Classic-duck',
                    price: 29,
                },
                {
                    img: 'product-item3.png',
                    avg: 5,
                    name: 'Bat-duck',
                    price: 69,
                },
            ],

        }
    }

}

</script>

<template>

    <div id="our-products">

        <h2>La collezione di paperelle</h2>

        <p>Una paperella per ogni stile di programmazione</p>
        
        <div class="product" v-for="actualProduct in products">

            <div class="duck-thumb">
                <img :src="'/images/' + actualProduct.img" alt="">
            </div>

            <div class="product-info">
                
                <div class="duck-avg">
                    <i class="fa-solid fa-star" v-for="n in actualProduct.avg"></i>
                </div>
    
                <div class="duck-name">
                    {{ actualProduct.name }}
                </div>
    
                <div class="duck-price">
                    ${{ actualProduct.price }}
                </div>

            </div>

        </div>

    </div>

</template>

<style lang="scss" scoped>
@use '../styles/variables' as *;

#our-products{
    margin-bottom: $margin-section;
    
    text-align: center;
    
    background-color: #F8F8F8;

    h2 {
        margin-bottom: 24px;
    }

    p {
        margin-bottom: 31px;

        font-size: .8em;
    }

    .product{
        display: flex;
        flex-direction: column;
        gap: 5px;

        padding: 0 5px;
        margin-bottom: 10px;

        text-align: start;

        .duck-thumb {

            img{
                width: 100%;
            }

        }

        .product-info{
            display: flex;
            flex-direction: column;
            gap: 5px;
            align-self: flex-start;
    
            .duck-avg {
                color: $avg-color;
            }
    
            .duck-price {
                font-weight: bold;
    
                color: $myGreen;
            }

        }

    }

}

</style>