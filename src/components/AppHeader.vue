<script>

export default{

    name: 'AppHeader',

}

</script>

<template>

    <nav>
        
        <div class="logo">
            <img src="/images/logo.png" alt="">
        </div>

        <div class="icon-menu">
            <div class="row first"></div>
            <div class="row second"></div>
            <div class="row third"></div>
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

    .icon-menu{
        display: flex;
        flex-direction: column;
        align-items: flex-end;
        gap: 4px;

        .row {
            height: 2px;

            border-radius: 2px;

            background-color: black;
        }

        .first {
            width: 22px;
        }
        .second {
            width: 15px;
        }

        .third {
            width: 8px;
        }
    }

}

</style>