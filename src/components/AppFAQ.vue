<script>

export default {

    name: 'AppFAQ',

    data() {
        return {

            faqs: [
                {
                    question: 'Come posso utilizzare la paperella di gomma per il debugging?',
                    answer: 'Il rubber duck debugging è semplice: spiega il tuo codice alla paperella di gomma come se fosse un collega. Descrivendo ogni passo, potresti individuare errori o capire meglio il problema. La paperella non risponde, ma ti aiuta a chiarire i tuoi pensieri.',
                },
                {
                    question: 'Quali sono i vantaggi di usare una paperella di gomma per i programmatori?',
                    answer: 'La paperella di gomma aiuta i programmatori a pensare in modo critico e a verbalizzare i problemi. Questo processo può portare a nuove intuizioni e soluzioni. Inoltre, è un ottimo strumento antistress e aggiunge un tocco di personalità alla scrivania.',
                },
                {
                    question: 'Posso usare la paperella di gomma indipendentemente dal linguaggio di programmazione che utilizzo?',
                    answer: 'Assolutamente sì! La paperella di gomma è universale e funziona con qualsiasi linguaggio di programmazione. Non importa se stai scrivendo in Python, Java, C++ o qualsiasi altro linguaggio, la paperella sarà sempre pronta ad ascoltarti.',
                },
                {
                    question: 'Quanto dettagliatamente devo spiegare il mio codice alla paperella di gomma?',
                    answer: 'Dovresti spiegare ogni dettaglio del tuo codice. Più sei dettagliato, più è probabile che tu scopra errori o ottenga nuove prospettive. Questo processo ti costringe a rivedere attentamente ogni parte del tuo lavoro.',
                },
            ],

        }
    }

}

</script>

<template>

    <div id="faq-section">

        <div class="faq-thumb">
            <img src="/images/single-image2.png" alt="">
        </div>

        <h2>FAQs</h2>

        <div class="faqs">

            <div class="faq" v-for="actualFaq in faqs">

                <div class="question">
                    <h4>{{ actualFaq.question }}</h4>
                    <i class="fa-solid fa-plus"></i>
                    <i class="fa-solid fa-minus"></i>
                </div>

                <div class="answer">
                    {{ actualFaq.answer }}
                </div>

            </div>

        </div>

    </div>

</template>

<style lang="scss" scoped>
@use '../styles/variables' as *;

#faq-section {

    padding: 0 5px;
    margin-bottom: $margin-section;

    .faq-thumb {

        img {
            width: 100%;
        }

    }

    h2 {
        margin-bottom: 30px;
    }
    
    .faqs {

        .faq {

            margin-bottom: 34px;

            .question {
                display: flex;
                justify-content: space-between;
                align-items: center;

                margin-bottom: 10px;

                .fa-plus {

                }

                .fa-minus {
                    display: none;
                }


            }

        }

    }

}

</style>