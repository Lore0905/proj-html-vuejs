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
                        <h5>ABOUT THE NETWORK</h5>
                        <h2><span class="the-company-section">The</span> Company</h2>
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
                        <h5>OUR BUSINESS AREAS</h5>
                        <!-- title -->
                        <h2>Excellence in <span>Services</span> </h2>
                        
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
            </div>
        </section>
        
    </main>
</template>

<script>
import Jumbotron from './Jumbotron.vue'
import Card from './Card.vue'
export default {
    name: 'Main',
    components: {
        Jumbotron,
        Card
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
            ]
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
                padding: 60px 0;

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
                    h5{
                        color: $color2;
                        font-size: 15px;
                    }
                    h2{
                        font-weight: 600;
                        font-size: 50px;
                        padding: 20px 0;
                        .the-company-section{
                            color: $color2;
                            background-color: rgba(3, 132, 131, 0.1);
                            padding: 10px 15px;
                            border-radius: 10px;
                        }
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
    // advantages
    .services{
        background-color: #111117;
        width: 100%;
        color: white;
        padding: 120px 0;
        .container{
            h5{
                font-size: 15px;
                color: $color2;
            }
            h2{
                font-size: 50px;
                font-weight: 900;
                margin: 1rem 0;
                span{
                    color: $color2;
                    background-color: rgba(3, 132, 131, 0.1);
                    padding: 10px 15px;
                    border-radius: 7px;
                }
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
}

</style>