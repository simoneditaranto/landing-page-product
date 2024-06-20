<script>

export default{

    name: 'AppHeader',

    data() {
        return {

            navLinks: [
                'Home',
                'I punti di forza',
                'Recensioni',
                'Paperelle',
                'FAQs',
                'NewsLetter',
            ],

        }
    }

}

</script>

<template>

    <nav>
        
        <div class="logo">
            <img src="/images/logo.png" alt="">
        </div>

        <div class="icon-menu">

            <svg class="icon">
                <use xlink:href="#navbar-icon"></use>
            </svg>

        </div>

        <div class="links">
                <ul>
                    <li v-for="link in navLinks">
                        {{ link }}
                    </li>
                </ul>
        </div>

    </nav>

</template>

<style lang="scss" scoped>

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 7px 15px 18px;

    .logo{

        width: 38px;
        height: 38px;

        img {
            width: 100%;
            height: 100%;
        }

    }

    .icon-menu {

        .icon {
            width: 30px;
            height: 30px;
        }

    }

    .links {

        ul {
            display: flex;
            gap: 20px;

            list-style-type: none;

            li {

                font-size: .9em;

            }
        }

    }

}

@media screen and (max-width: 768px) {

    .links {
        display: none;
    }

}

@media screen and (min-width: 769px) {

    .icon-menu {
        display: none;
    }


}

</style>