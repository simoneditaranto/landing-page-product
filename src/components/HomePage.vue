<script>

export default {

    name: 'HomePage',
    
    data() {
        return {

            info: [
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
            ],

        }
    }

}

</script>

<template>

    <div class="info">
        <div class="description" v-for="(actualInfo, index) in info">
            <h3 class="title">{{ actualInfo.title }}</h3>
            <div class="text">{{ actualInfo.text }}</div>
            <div class="duck-point" v-if="index == 2">
                <!-- <img src="/images/invisible.png" alt=""> -->
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>

.info{
    display: flex;
    flex-direction: column;
    gap: 32px;

    padding: 5px;
    margin-bottom: 20px;

    text-align: center;

    .description{

        .title{
            margin-bottom: 8px;
        }

        .duck-point{
            margin-top: 32px;

            height: 332px;

            background-image: url('/images/invisible.png');
            background-size: cover;
            background-position: top;
        }

    }

}


</style>