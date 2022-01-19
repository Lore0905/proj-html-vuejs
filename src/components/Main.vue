<template>
    <main>

        <!-- jumbotron -->
        <div class="jumbotron">
            <Jumbotron/>
        </div>

        <!-- card -->
        <section class="advatages">
            <div class="container">
                <div class="wrapping-card">
                    <Card v-for="(advantage, index) in advantages" :key="index" :cardDetails="advantage" type="advantage"/>
                </div>
            </div>
        </section>

        <!-- company section -->
        <section class="company-section">
            <div class="row">
                <div class="col-6 col-sx-company">

                    <!-- wrapping text -->
                    <div class="wrapping-text">
                        <h5 class="title-area">ABOUT THE NETWORK</h5>
                        <h2><span class="word-enfasi">The</span> Company</h2>
                        <p>For 12 years we have been providing audit and warranty, financial advice, taxes and related services to select clients.</p>

                        <div class="row">

                            <!-- COL -->
                            <div class="col-6">
                                <!-- title with icon -->
                                <h4>
                                    <i class="fas fa-medal"></i>
                                    Tradition
                                </h4>
                                <!-- description  -->
                                <p>
                                    Lorem ipsum dolor, sit amet consectetur adipisicing 
                                </p>
                            </div>

                            <!-- COL -->
                            <div class="col-6">
                                <!-- title with icon -->
                                <h4>
                                    <i class="fas fa-lock"></i>
                                    Security
                                </h4>
                                <!-- description  -->
                                <p>
                                    Lorem ipsum dolor, sit amet consectetur adipisicing 
                                </p>
                            </div>

                            <!-- COL -->
                            <div class="col-6">
                                <!-- title with icon -->
                                <h4>
                                    <i class="fas fa-file-signature"></i>
                                    Certificate
                                </h4>
                                <!-- description  -->
                                <p>
                                    Lorem ipsum dolor, sit amet consectetur adipisicing 
                                </p>
                            </div>

                            <!-- COL -->
                            <div class="col-6">
                                <!-- title with icon -->
                                <h4>
                                    <i class="fas fa-graduation-cap"></i>
                                    Expertise
                                </h4>
                                <!-- description  -->
                                <p>
                                    Lorem ipsum dolor, sit amet consectetur adipisicing 
                                </p>
                            </div>
                            
                        </div>
                    </div>

                </div>
                <!-- COL -->
                <div class="col-6">
                    <img src="../assets/about-3.jpg" alt="about-3">
                </div>

                <!-- SERVICES -->
                <section class="services">
                    <div class="container">
                        <!-- small title -->
                        <h5 class="title-area">OUR BUSINESS AREAS</h5>
                        <!-- title -->
                        <h2>Excellence in <span class="word-enfasi">Services</span> </h2>
                        
                        <div class="row">
                            <div class="col-9">
                                <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of experienced and renowned professional. Theese are some options that you can hire.</p>
                            </div>
                            <div class="col-3">
                                <!-- button -->
                                <div class="btn second-btn">
                                    <button>SEE ALL</button>
                                </div>
                            </div>  

                        </div>

                        <div class="wrapping-card">
                            <Card v-for="(service, index) in services" :key="index" :cardDetails="service" type="service"/>
                        </div>
                    </div>
                </section>


                <!-- PRICING SECTION -->
                <section class="pricing-table">
                    <div class="container">
                        <!-- title area -->
                        <h5 class="title-area">MONTHLY PLANS</h5>
                        <!-- title -->
                        <h2><span class="word-enfasi">Pricing</span>Table</h2>
                        <!-- paragrafo -->
                        <p>We can help you deliver and execute your future, wherever you compete, using the latest <br> technologies, from strategy development to implementation</p>

                        <!-- RAW -->
                        <div class="row">
                            <!-- COL -->
                            <div class="col-4">

                                <div class="wrapping-table">
                                    <!-- img -->
                                    <div class="logo-table">
                                        <i class="fas fa-rocket"></i>
                                    </div>
                                    <!-- title -->
                                    <h4>Standard</h4>
                                    <!-- price -->
                                    <div class="price">
                                        <span class="simbol">$</span>
                                        <span class="number">490</span>
                                        <span> / mo</span>
                                    </div>
                                    <!-- list services -->
                                    <table>
                                        <tbody>
                                            <tr class="row">
                                                <td class="col-8">Standar Accounting</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Platform Access</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Business Orientation</td>
                                                <td class="col-4"><i class="fas fa-times"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Dedicated Consultant</td>
                                                <td class="col-4"><i class="fas fa-times"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Personal Assistance</td>
                                                <td class="col-4"><i class="fas fa-times"></i></td>
                                            </tr>
                                        </tbody>
                                    </table>
                                </div>

                            </div>

                            <!-- COL -->
                            <div class="col-4 popular-price">

                                <div class="wrapping-table">
                                    <!-- img -->
                                    <div class="logo-table">
                                        <i class="fas fa-suitcase"></i>
                                    </div>
                                    <!-- title -->
                                    <h4>Professional</h4>
                                    <!-- price -->
                                    <div class="price">
                                        <span class="simbol">$</span>
                                        <span class="number">890</span>
                                        <span> / mo</span>
                                    </div>
                                    <!-- list services -->
                                    <table>
                                        <tbody>
                                            <tr class="row">
                                                <td class="col-8">Standar Accounting</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Platform Access</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Business Orientation</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Dedicated Consultant</td>
                                                <td class="col-4"><i class="fas fa-times"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Personal Assistance</td>
                                                <td class="col-4"><i class="fas fa-times"></i></td>
                                            </tr>
                                        </tbody>
                                    </table>
                                </div>

                                <!-- etichetta most popular -->
                                <div class="label-price-popular">
                                    Most<br>Popular
                                </div>

                            </div>

                            <!-- COL -->
                            <div class="col-4">

                                <div class="wrapping-table">
                                    <!-- img -->
                                    <div class="logo-table">
                                        <i class="far fa-gem"></i>
                                    </div>
                                    <!-- title -->
                                    <h4>Ultimate</h4>
                                    <!-- price -->
                                    <div class="price">
                                        <span class="simbol">$</span>
                                        <span class="number">1.390</span>
                                        <span> / mo</span>
                                    </div>
                                    <!-- list services -->
                                    <table>
                                        <tbody>
                                            <tr class="row">
                                                <td class="col-8">Standar Accounting</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Platform Access</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Business Orientation</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Dedicated Consultant</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                            <tr class="row">
                                                <td class="col-8">Personal Assistance</td>
                                                <td class="col-4"><i class="fas fa-check"></i></td>
                                            </tr>
                                        </tbody>
                                    </table>
                                </div>

                            </div>

                        </div>
                    </div>
                </section>

                <!-- latest news -->
                <section class="latest-news">
                    <div class="container">

                        <!-- title-area -->
                        <div class="title-area">OUR EDITORIAL CONTENT</div>
                        <!-- title -->
                        <h2>Latest <span class="word-enfasi">News</span></h2>

                        <!-- ROW -->
                        <div class="row">

                            <!-- COL -->
                            <div class="col-9">
                                <!-- paragrafo -->
                                <p>Every we publish content about what is best in the business world.</p>
                            </div>

                            <!-- COL -->
                            <div class="col-3">
                                <div class="btn second-btn">
                                    <button>SEE ALL</button>
                                </div>
                            </div>

                        </div>
                        
                        <div class="wrapping-cards-news">
                            <CardNews v-for="(news, index) in CardNews" :key="index" :details="news"/>
                        </div>
                    </div>
                </section>


                <!-- news letter -->
                <section class="newsletter-wrapping">
                    <div class="container">
                        <div class="row">

                            <!-- col -->
                            <div class="col-6">
                                 <!-- title area -->
                                <div class="title-area">
                                    NEWSLETTER
                                </div>
                                <!-- title -->
                                <h2><span class="word-enfasi">Know</span> First</h2>
                                <!-- paragrafo -->
                                <p>Follow closely and receive content about our company and the news of the current market.</p>
                            </div>

                            <!-- col -->
                            <div class="col-6">
                                <!-- input -->
                                <div class="wrapping-input">
                                    <input type="text" placeholder="Name">
                                    <input type="email" placeholder="Email">
                                </div>
                                <!-- button -->
                                <div class="btn second-btn p-0">
                                    <button>SUBSCRIBE</button>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>

                <!-- send a mesage -->
                <section class="message-wrapping">
                    <div class="container">
                        <div class="row">

                            <!-- col -->
                            <div class="col-8">

                                <!-- text -->
                                <div class="text-message-section">
                                    <!-- title area -->
                                    <div class="title-area">
                                        SEND A MESSAGE
                                    </div>
                                    <!-- title -->
                                    <h2>Get in <span class="word-enfasi">Touch</span></h2>
                                    <!-- paragrafo -->
                                    <p>We will respond to your message as soon as possible.</p>
                                </div>

                                <!-- input -->
                                <div class="input-message-section">
                                    <input type="text" placeholder="Name">
                                    <input type="email" placeholder="Email">
                                    <input type="text" placeholder="Phone">
                                    <input type="text" placeholder="More Info">
                                    <div>
                                        <textarea name="" id="text-area-message" placeholder="Message"></textarea>
                                    </div>
                                </div>

                                <!-- button -->
                                <div class="btn second-btn p-0">
                                    <button>SEND</button>
                                </div>
                            </div>

                            <!-- col -->
                            <div class="col-4">
                                ciao
                            </div>
                        </div>
                    </div>
                </section>

            </div>
        </section>
        
    </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import Card from './Card.vue'
import CardNews from './CardNews.vue'
export default {
    name: 'Main',
    components: {
        Jumbotron,
        Card,
        CardNews
    },
    data: function(){
        return{
            advantages: [
                {
                    title: 'Human Capital',
                    paragrafo: 'Humanizing business: Harness the power of technology to improve the way people work.',
                    class: 'fas fa-user-friends'
                },
                {
                    title: 'Core Business',
                    paragrafo: 'It takes innovative approaches to transform, and run existing platforms.',
                    class: 'fas fa-chart-pie'
                },
                {
                    title: 'Perforamnce',
                    paragrafo: 'Archieving maximum impact and value from investements in finance and supply chain.',
                    class: 'fas fa-tachometer-alt'
                }
            ],
            services: [
                {
                    title: 'Audit & Assurance',
                    paragrafo: 'Lorem ipsum dolor, sit amet consectetur adipisicing .',
                    class: 'fas fa-project-diagram'
                },
                {
                    title: 'Financial Advisory',
                    paragrafo: 'Lorem ipsum dolor, sit amet consectetur adipisicing .',
                    class: 'fas fa-suitcase' 
                },
                {
                    title: 'Analitics and M&A',
                    paragrafo: 'Lorem ipsum dolor, sit amet consectetur adipisicing .',
                    class: 'fas fa-chart-bar' 
                },
                {
                    title: 'Middle Marketing',
                    paragrafo: 'Lorem ipsum dolor, sit amet consectetur adipisicing .',
                    class: 'fas fa-plane' 
                },
                {
                    title: 'Legal Consulting',
                    paragrafo: 'Lorem ipsum dolor, sit amet consectetur adipisicing .',
                    class: 'fas fa-globe-asia' 
                },
                {
                    title: 'Regolatory Risk',
                    paragrafo: 'Lorem ipsum dolor, sit amet consectetur adipisicing .',
                    class: 'fas fa-box' 
                }
            ],
            CardNews: [
                {
                    title: 'Increasing creativity is possible for everyone',
                    paragrafo: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit.',
                    author: 'Andrea Miller',
                    img: 'news-1'
                },
                {
                    title: 'Becouse Market reserch is part of the business plan',
                    paragrafo: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit.',
                    author: 'Andrea Miller',
                    img: 'news-2'
                },
                {
                    title: 'Working from home is now a trend',
                    paragrafo: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit.',
                    author: 'Andrea Miller',
                    img: 'news-3'
                }
            ],
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
main{
    // jumbotron

    // advantages
    .advatages{
        background-color: $color3;
        width: 100%;
        .container{
            .wrapping-card{
                display: flex;
                flex-wrap: wrap;
                padding: $paddingsection;

            }
        }
    }
    // company section
    .company-section{

        .row{

            .col-sx-company{
                display: flex;
                justify-content: end;
                align-items: center;

                .wrapping-text{
                    width: 55%;
                    h2{
                        padding: 20px 0;
                    }
                    p{
                        color: #778a94;
                        font-weight: 200;
                        font-size: 17px;
                    }
                    .row{
                        padding: 30px 0px;
                        .col-6{
                            padding-bottom: 30px;
                            h4{
                                padding: 10px 0;
                                i{
                                    color: $color2;
                                }
                            }
                            
                        }
                    }
                }

            }
        }
    }

    // SERVICES
    .services{
        background-color: #111117;
        width: 100%;
        color: white;
        padding: $paddingsection;
        .container{
            h2{
                margin: 1rem 0;
            }
            .row{
                align-items: baseline;
            }
            .wrapping-card{
                display: flex;
                flex-wrap: wrap;
                padding: 60px 0;

            }
        }
    }

    // PRICING
    .pricing-table{
        background-color: $color3;
        padding: $paddingsection;
        text-align: center;
        .container{
            h5{
                padding: 25px 0;
            }
            p{
                font-size: 17px;
                padding: 25px 0;
                color: $grey;
            }
            .row{
                .col-4{
                    .wrapping-table{
                        background-color: white;
                        border-radius: 10px;
                        padding: 50px;
                        font-size: 17px;
                        position: relative;
                        .logo-table{
                            font-size: 50px;
                            color: $color2;
                        }
                        .price{
                            color: $color2;
                            padding: 10px 0;
                            .simbol{
                                font-size: 25px;
                            }
                            .number{
                                font-size: 40px;
                                font-weight: 500;
                            }
                        }
                        h4{
                            font-weight: 500;
                            font-size: 27px;
                        }
                        table{
                            width: 100%;
                            text-align: left;
                            color: $grey;
                            .col-8{
                                padding: 10px 0;
                            }
                            .col-4{
                                padding: 10px 0;
                                text-align: right;
                                color: $color2;
                            }
                        }
                    }
                    .label-price-popular{
                        padding: 7px 15px;
                        border-radius:  0 10px 10px 0;
                        background-color: $color2;
                        display: inline-block;
                        position: absolute;
                        top: 10px;
                        left: 12px;
                        font-size: 13px;
                        text-align: left;
                        line-height: 13px;
                        color: white;
                    }

                }
            }
        }
    }
    // dinamiche
    .popular-price{
        transform: scaleY(1.07);
    }
    // LATEST NEWS
    .latest-news{
        padding: $paddingsection;
        .container{
            h2{
                padding: 20px 0;
            }
            .row{
                align-items: baseline;
                .col-9{
                    color: $grey;
                }
                .col-3{
                    .second-btn{
                        background-color: $color2;
                    }
                }
            }
            .wrapping-cards-news{
                padding: 50px 0;
                display: flex;
                justify-content: space-between;
            }
        }
    }

    // NEWS LETTER
    .newsletter-wrapping{
        width: 100%;
        height: 500px;
        background-image: url(../assets/bg-1.jpg);
        background-position-y: center;
        background-size: cover;
        color: white;
        .container{
            width: 100%;
            height: 100%;
            padding: 100px;
            .row{
                width: 100%;
                height: 100%;
                align-items: center;
                .col-6{
                    // col-sx
                    h2{
                        padding: 12px 0;
                        .word-enfasi{
                            color: white;
                        }
                    }
                    p{
                        color: $grey;
                    }
                    // col-dx
                    .wrapping-input{
                        margin: 10px 0;
                        input{
                            width: 80%;
                            border-radius: 5px;
                            border: 0px;
                            background-color: rgba($color: #ffffff, $alpha: 0.5);
                            padding: 12px;
                            margin: 10px 0;
                        }
                    }
                    .second-btn{
                        button{
                            background-color: $color2;
                        }
                    }
                }
                
            }
        }
    }

    // message
    .message-wrapping{
        padding: $paddingsection;
        .container{
            .row{
                .col-8{
                    .input-message-section{
                        input{
                            width: calc(50% - 10px);
                            border-radius: 5px;
                            border: 0px;
                            background-color: rgba($color: #8d8f92, $alpha: 0.2);
                            padding: 12px;
                            margin: 10px 0px;
                        }
                        input:nth-child(odd){
                            margin-right: 20px;
                        }
                        div{
                            #text-area-message{
                                width: 100%;
                                height: 150px;
                                border-radius: 5px;
                                min-height: 50px;
                                max-height: 250px;
                                border: 0px;
                                padding: 12px;
                                margin-top: 10px;
                                background-color: rgba($color: #8d8f92, $alpha: 0.2);
                            }
                        }
                    }
                }
                .second-btn{
                    margin-top: 10px;
                    button{
                        background-color: $color2;
                    }
                }
            }
        }
    }

}







</style>