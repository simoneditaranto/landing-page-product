<script>

export default {

    name: 'HomePage',
    
    data() {
        return {

            firstInfo: [
                {
                    title: 'Lunga durata della batteria',
                    text: 'Godidi ore di assistenza continua nella risoluzione di bug grazie alla lunga durata della "battaeria" (ovver, la tua pazienza) della paperella di gomma.',
                },
                {
                    title: 'Compatibilità Universale',
                    text: 'Funziona con tutti i linguaggi di programmazione e sistemi operativi, la paperella di gomma è l unico strumento di debugging che non necessita di aggiornamenti.',
                },
                {
                    title: 'Design Elegante',
                    text: 'Mostra con orgoglio il design elegante e raffinato della tua paperella di gomma, disponibile in vari colori per abbinarsi al tuo stile di programmatore.',
                },
            ],

            secondInfo: [
            {
                    title: 'Resistenza agli Spruzzi',
                    text: 'Perfetta per resistere ai piccoli incidenti con caffè e bevande, la tua paperella di gomma non teme schizzi, mantenedoti sempre pronto per il debugging.',
                },
                {
                    title: 'Portabilità',
                    text: 'Leggera e facile da trasportare, la paperella di gomma può essere il tuo compagno di lavoro ovunque tu vada. Portala con te per un supporto costante.',
                },
                {
                    title: 'Promemoria Anti-Stress',
                    text: 'Quando lo stress del codice diventa troppo, spremi la tua paperella per un rapido sollievo anti-stress, senza bisogno di software complicati.',
                },
            ]


        }
    }

}

</script>

<template>

    <div class="info">

        <div class="start">

            <div class="description"    v-for="actualInfo in firstInfo">
                <h3 class="title">{{ actualInfo.title }}</h3>
                <div class="text">{{ actualInfo.text }}</div>
            </div>

        </div>

        <div class="middle">

            <div class="duck-point">
                <img src="/images/invisible.png" alt="">
            </div>

        </div>

        <div class="start">

            <div class="description"    v-for="actualInfo in secondInfo">
                <h3 class="title">{{ actualInfo.title }}</h3>
                <div class="text">{{ actualInfo.text }}</div>
            </div>

        </div>

    </div>

</template>

<style lang="scss" scoped>
@use '../styles/variables' as *;

.info{
    display: flex;
    flex-direction: column;
    gap: 32px;

    padding: 5px;
    margin-bottom: $margin-section;

    text-align: center;

    .start {
        display: flex;
        flex-direction: column;
        gap: 32px;

        .description{
    
            .title{
                margin-bottom: 8px;
            }
            
        }

    }

    
    .duck-point{

        margin-top: 32px;

        img {
            width: 100%;
            // height: 100%;
            object-fit: cover;
            object-position: top;
        }

    }
}

@media screen and (min-width: 769px) {

    .info {
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
    }

    // .duck-point {
    //     max-width: 350px;

    //     img {
    //     }

    // }


}


</style>