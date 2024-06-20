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
            ],

        }
    }

}

</script>

<template>

    <div class="info">
        <div class="description" v-for="actualInfo in info">
            <h3 class="title">{{ actualInfo.title }}</h3>
            <div class="text">{{ actualInfo.text }}</div>
        </div>
    </div>

</template>

<style lang="scss" scoped>

.info{
    display: flex;
    flex-direction: column;
    gap: 32px;

    padding: 5px;

    text-align: center;

    .description{

        .title{
            margin-bottom: 8px;
        }
        
    }

}


</style>