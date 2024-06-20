<script>

export default {

    name: 'ContactUs',

    data() {
        return {

            socials: [
                'facebook',
                'twitter',
                'youtube',
                'linkedin',
                'instagram',
            ]

        }
    }

}

</script>

<template>

    <div id="contact-us">

        <h2>Iscrivi per rimanere aggiornato</h2>

        <p>Iscriviti alla nostra newsletter per rimanere aggiornato</p>

        <div class="mail">
            <input type="text" placeholder="Lascia la tua email qui">

            <svg class="icon">
                <use xlink:href="#send"></use>
            </svg>
        </div>

        <div class="socials">

            <div class="social" v-for="social in socials">

                <svg class="icon">
                    <use :xlink:href="'#' + social"></use>
                </svg>

            </div>
            
        </div>

    </div>

</template>

<style lang="scss">
@use '../styles/variables' as *;

#contact-us {
    padding: 17px 12px;

    text-align: center;

    background-color: #F8F8F8;

    h2 {
        margin-bottom: 18px;
    }

    p {
        margin-bottom: 40px;

        font-size: .8em;
    }

    .mail {
        display: flex;
        justify-content: space-between;
        align-items: center;

        margin-bottom: 28px;

        border-bottom: 1px solid #DEE2E6;

        input {
            flex-grow: 1;

            padding: 10px 0;

            border: none;

            background-color: #F8F8F8;

        }

        .icon {
            width: 24px;
            height: 24px;
            color: $myGreen; /* Colore dell'icona */
        }
    }

    .socials {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 10px;

        .social {
            width: 40px;
            height: 40px;
    
            border: 1px solid #DEE2E6;
            border-radius: 50%;
    
            .icon {
                width: 20px;
                height: 100%;
                color: $myGreen;
            }
        }
    }

}

</style>