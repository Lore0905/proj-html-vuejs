<template>
    <header>
        <!-- CONTACTS -->
        <section class="contact">

        </section>

        <!-- NAV -->
        <section class="nav">
            <div class="container">

                <!-- logo -->
                <div id="logo">
                    logo
                </div>

                <!-- link -->
                <div id="link-header">
                    link
                    link
                    link
                    link
                    link
                    link
                    link
                </div>

            </div>
        </section>
    </header>
</template>

<script>
export default {
    name: 'Header'
}
</script>

<style lang="scss">
header{
    .contact{
        width: 100%;
        height: 40px;
        background-color: #24333d
    }
    .nav{
        position: relative;
        z-index: 1;

        .container{
            display: flex;
            position: absolute;
            top: 0px;
            left: 50%;
            transform: translate(-50%);
            #logo{
                flex-grow: 1;
            }
        }
    }
}
</style>