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
                    <h2><span class="nex">NEX</span><span>GEN</span></h2>
                </div>

                <!-- link -->
                <div id="link-header">

                    <ul>
                        <li>
                        <a href="#">link</a>
                        </li>
                        <li>
                            <a href="#">link</a>
                        </li>
                        <li>
                            <a href="#">link</a>
                        </li>
                        <li>
                            <a href="#">link</a>
                        </li>
                    </ul>
                    
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
@import '../style/variables.scss';
header{
    color: white;
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
            align-items: center;
            position: absolute;
            top: 0px;
            left: 50%;
            transform: translate(-50%);
            padding: 20px 0px;

            #logo{
                flex-grow: 1;
                h2{
                    font-size: 25px;
                    font-weight: 500;
                    letter-spacing: 7px;
                    .nex{
                        background-color: rgba(3, 132, 131, 0.5);
                        color: $color1;
                        padding: 10px 0;
                        padding-left: 30px;
                        border-radius: 30px 0 0 30px;
                    }
                }
            }
            #link-header{
                ul{
                    li{
                        padding: 10px;
                        display: inline-block;
                    }
                }
            }
        }
    }
}
</style>