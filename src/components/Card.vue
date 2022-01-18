<template>


    <div class="container-card white">
        <!-- logo -->
        <div class="circle h-v-center">
            <i class="icon" :class='singleAdvantage.class'></i>
        </div>
        <!-- title -->
        <div class="title">
            <h4>{{singleAdvantage.title}}</h4>
        </div>
        <!-- paragrafo -->
        <div>
            <p>{{singleAdvantage.paragrafo}}</p>
        </div>
    </div>


</template>


<script>
export default {
    name: "Card",
    props: ['singleAdvantage']
}
</script>

<style lang="scss">
@import '../style/variables.scss';

.container-card{
    width: calc((100% / 3) - 20px);
    padding: 40px 50px;
    border-radius: 7px;
    margin:10px;
    .circle{
        border-radius: 50%;
        width: 60px;
        height: 60px;
        .icon{
            color: $color2;
            font-size: 30px;
        }
    }
    .title{
        padding: 20px 0;
        h4{
            font-weight: 500;
        }
    }
    p{
        color: $grey;
        font-size: 18px;
    }
}

// classi dinamiche
.white{
    background-color: white;
}
.circle{
    
    background-color: $color3;
}
</style>