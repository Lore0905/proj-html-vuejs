<template>


    <div class="container-card" :class=" type === 'advantage' ? 'white' : 'grey'">
        <!-- logo -->
        <div class="circle h-v-center" :class="type === 'advantage' ? 'circle-advantage' : 'circle-service'">
            <i class="icon" :class='cardDetails.class'></i>
        </div>
        <!-- title -->
        <div class="title" >
            <h4>{{cardDetails.title}}</h4>
        </div>
        <!-- paragrafo -->
        <div>
            <p>{{cardDetails.paragrafo}}</p>
        </div>
        <!-- button -->
        <div class="btn second-btn p-0" v-if="type === 'service'">
            <button>READ MORE</button>
        </div>
    </div>


</template>


<script>
export default {
    name: "Card",
    props: 
    {
        cardDetails: Object, 
        type: String
    }
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
            font-size: 27px;
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
.grey{
    background-color: #19191f;
    color: white;
}
.circle-advantage{
    background-color: $color3;
}
.circle-service{
    background-color: #19191f;
}
</style>