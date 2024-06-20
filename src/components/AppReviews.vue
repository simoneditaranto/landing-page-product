<script>

export default {

    name: 'AppReviews',

    data() {
        return {

            reviewsList: [
                {
                    text: 'La paperella di gomma è diventata il mio strumento di debugging preferito. Spiegare i problemi al mio "assistente" silenzioso mi ha aiutato a risolvere bug che altrimenti mi avrebbero fatto impazzire. È anche un ottimo antistress nelle giornate difficili!',
                    author: 'David William',
                    date: 'Feb 22, 2023',
                },
                {
                    text: 'Non avrei mai immaginato quanto una semplice paperella di gomma potesse fare la differenza. È incredibile come verbalizzare i problemi davanti alla paperella mi aiuti a vedere soluzioni che prima non notavo. Inoltre, è carinissima sulla mia scrivania!',
                    author: 'Emma Turner',
                    date: 'April 5, 2023',
                },
                {
                    text: 'Da quando ho adottato la paperella di gomma, il mio processo di debugging è migliorato notevolmente. La trovo molto utile per schiarirmi le idee e trovare errori nascosti. La porto sempre con me, ovunque vada!',
                    author: 'Rachel Bryan',
                    date: 'April 18, 2023',
                },
                {
                    text: 'La mia paperella di gomma è il miglior collega che potessi chiedere. Sempre pronta ad ascoltare, mai giudicante. È sorprendente come qualcosa di così semplice possa essere così efficace nel risolvere problemi complessi. E non dimentichiamo che è anche adorabile!',
                    author: 'Park C',
                    date: 'May 22, 2023',
                },
            ],

            actualSlide: 0,

        }
    }

}

</script>

<template>

    <div id="reviews">

        <h2>Cosa ne pensano i nostri sviluppatori</h2>

        <div class="review">

            <div class="text">
                "La paperella di gomma è diventata il mio strumento di debugging preferito. Spiegare i problemi al mio "assistente" silenzioso mi ha aiutato a risolvere bug che altrimenti mi avrebbero fatto impazzire. È anche un ottimo antistress nelle giornate difficili!"
            </div>

            <div class="review-avg">
                <i class="fa-solid fa-star" v-for="n in 5"></i>
            </div>

            <div class="review-info">
                Park C - May 22, 2023
            </div>

        </div>

        <div class="slider">

            <div 
                class="count-slider" 
                v-for="(n, index) in reviewsList" 
                :class="actualSlide == index ? 'selected' : ''" 
                @click="actualSlide = index"
            >
            </div>

        </div>


    </div>

</template>

<style lang="scss" scoped>
@use '../styles/variables' as *;

#reviews{

    margin-bottom: 20px;

    text-align: center;

    h2{
        margin-bottom: 27px;
    }

    .review {

        margin-bottom: 18px;

        .text{
            margin-bottom: 16px;
        }

        .review-avg{
            margin: 11px;

            color: #FFC10A;
        }

        .review-info{
            font-weight: bold;
        }

    }

    .slider{
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 5px;

        .count-slider{
            width: 15px;
            height: 15px;
    
            border-radius: 50%;
    
            background-color: #CCCCCC;
        }

        .count-slider.selected{
            background-color: $myBlue;
        }
    }


}


</style>