<script>

export default {

    name: 'AppJumbo',

}

</script>

<template>

    <div id="jumbotron">

        <div class="back-jumbo">
            <img src="/images/banner-image.png" alt="">
        </div>

        <div class="jumbo-banner">
            <h1>
                Rubber Duck Debugging
            </h1>

            <p>
                Spiegare il codice ad una paperella di gomma aiuta i programmatori a chiarire il pensieri e individuare errori nascosti.
            </p>

            <div class="button">
                Acquistala subito!
            </div>
        </div>

    </div>


</template>

<style lang="scss" scoped>
@use '../styles/variables' as *;

#jumbotron {
    display: flex;
    flex-direction: column;

    margin-bottom: $margin-section;

    .back-jumbo{
        
        img {
            width: 100%;
            // height: 100%;
            // object-fit: cover;
            // object-position: bottom;
            display: block;
        }

    }

    .jumbo-banner {
        
        padding: 47px 47px 27px;

        text-align: center;

        background-image: url('/images/banner-bg.png');

        h1 {
            margin-bottom: 18px;
        }

        p{
            margin-bottom: 25px;
        }

        .button {
            padding: 14px 24px;

            border: 1px solid black;

            // font-weight: bold;

            text-transform: uppercase;
        }

    }

}

@media screen and (min-width: 769px) {

    #jumbotron {
        flex-direction: row;

        .button{
            color: white;

            background-color: $myBlack;
        }
    }

}

</style>