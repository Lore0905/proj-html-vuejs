<template>
    <div>
        <!-- footer top -->
        <section class="footer-top">
            <div class="container">

                <!-- row -->
                <div class="row">
                    <!-- col -->
                    <div class="col-3 static">
                        <!-- logo -->
                        <div id="logo">
                            <h2><span class="nex">NEX</span><span>GEN</span></h2>
                        </div>
                        <!-- paragrafo -->
                        <p>A functional HTML Template for Corporate & Business.</p>
                        <!-- references -->
                        <div>
                            <ul class="p-0">
                                <li>
                                    <div>
                                        <i class="fas fa-phone-alt"></i>
                                    </div>
                                    <!-- number -->
                                    <div class="text">
                                        +1 (305) 1234-5678
                                    </div>
                                </li>
                                <li>
                                    <div>
                                        <i class="fas fa-envelope"></i>
                                    </div>
                                    <!-- email -->
                                    <div class="text">
                                        hello@example.com
                                    </div>
                                </li>
                                <li>
                                    <div>
                                        <i class="fas fa-map-marker-alt"></i>
                                    </div>
                                    <!-- number -->
                                    <div class="text">
                                        Main Avenue, 987
                                    </div>
                                </li>
                            </ul>
                        </div>
                        <!-- button -->
                        <div class="btn second-btn">
                            <button>GET IN TOUCH</button>
                        </div>
                    </div>
                    <!-- col -->
                    <div class="col-3" v-for="(card, index) in links" :key="index">
                        <div class="wrapping-col-dinamic">
                            <h2>{{card.title}}</h2>
                            <ul class="p-0">
                                <li v-for="(link, index) in card.link" :key="index">
                                    <i class="fas fa-chevron-right"></i>
                                    <a href="#">{{link}}</a>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- footer booton -->
        <section class="footer-bottom">
            <div class="container">
                <div class="row">
                    <!-- col -->
                    <div class="col-6">
                        Enjoy the low price. We are tracking any intention of piracy.
                    </div>
                    <!-- col -->
                    <div class="col-6 text-end">
                        2020 NEXGEN is Proudly Powered by <span class="title-area">Coding</span>
                    </div>

                </div>
            </div>
        </section>
    </div>
</template>

<script>
export default {
    name: 'Footer',
    props: ['links']
}
</script>

<style lang="scss">
@import '../style/variables.scss';
div{
    font-weight: 200;
    .footer-top{
        background-color: #111117;
        padding: $paddingsection;
        color: $grey;
        .col-3{
            p{
                padding: 20px 0;
            }
            ul{
                font-size: 17px;
                li{
                    display: flex;
                    margin-bottom: 10px;
                    align-items: center;
                    i{
                        margin-right: 10px;
                    }
                }
            }
            .btn{
                padding: 10px 0;
            }
            .wrapping-col-dinamic{
                background-color: rgba($color: #19191f, $alpha: 1);
                padding: 40px;
                border-radius: 10px;
                h2{
                    color: white;
                    font-size: 24px;
                    margin-bottom: 15px;
                }
            }
        }
    }
    .footer-bottom{
        background-color: #0d0c11;
        padding: 30px;
        color: $grey;
    }
}

</style>