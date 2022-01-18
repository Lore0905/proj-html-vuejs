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
                    <Card v-for="(advantage, index) in advantages" :key="index" :singleAdvantage="advantage"/>
                </div>
            </div>
        </section>
        <!-- company section -->
        <section class="company-section">
            <div class="raw">
                <div class="col-6">
                    ciaqo
                </div>
                <div class="col-6">
                    ciao
                </div>
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
                },
                {
                    title: 'Core Business',
                    paragrafo: 'It takes innovative approaches to transform, and run existing platforms.'
                },
                {
                    title: 'Perforamnce',
                    paragrafo: 'Archieving maximum impact and value from investements in finance and supply chain.'
                }
            ]
        }
    }
}
</script>

<style lang="scss">
@import '../style/variables.scss';
main{
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
    .company-section{
        .raw{
            display: flex;
            .col-6{
                // test
                border: 1px solid black;
            }
        }
    }
}

</style>