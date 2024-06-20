<script>

export default {

    name: 'AppInfo',

    data() {
        
        return {

            info: [
                {
                    icon: 'balloon',
                    title: '100% Prodotto di qualità',
                    text: 'Abbiamo anche la possibilità di ritiro diretto dallo stagno',
                },
                {
                    icon: 'bag-heart',
                    title: 'Spedizione gratuita',
                    text: 'Dal magazzi alla scrivania',
                },
                {
                    icon: 'handiplast',
                    title: 'Rimborso garantito',
                    text: 'Ti rimborsiamo se la paperella fa quack',
                },
            ],

        }

    }

}

</script>

<template>

    <div id="info">

        <div class="info-element" v-for="actualInfo in info">

            <svg class="icon">
                <use :xlink:href="'#' + actualInfo.icon"></use>
            </svg>

            <h4 class="title">
                {{ actualInfo.title }}
            </h4>

            <p class="text">
                {{ actualInfo.text }}
            </p>

        </div>
        
    </div>

</template>

<style lang="scss" scoped>
@use '../styles/variables' as *;

#info {

    text-align: center;

    .info-element {

        margin-bottom: 25px;

        .icon {
            width: 24px;
            height: 24px;
            color: $myBlue; /* Colore dell'icona */
        }

        .title {
            margin-bottom: 5px;
        }

        .text {
            font-size: .7em;
        }
    }


}

</style>