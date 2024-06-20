<script>

export default {

    name: 'AppJumbo',

}

</script>

<template>

    <div id="jumbotron">

        <div class="back-jumbo"></div>

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

#jumbotron {
    display: flex;
    flex-direction: column;

    margin-bottom: 20px;

    .back-jumbo{
        height: 255px;

        background-image: url('/images/banner-image.png');
        background-size: cover;
        background-position: bottom;
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

            font-weight: bold;

            text-transform: uppercase;
        }

    }

}

</style>