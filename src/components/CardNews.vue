<template >
    <div class="card-news-wrapping">

        <div class="background-img">
            <img :src="require('../assets/' + details.img + '.jpg')" alt="details.title">
        </div>

        <div class="text">

            <div class="row">

                <!-- col -->
                <div class="col-6">
                    <div class="hover-appears">
                        <div>
                            <i class="fas fa-user-alt"></i>
                        </div>
                        <!-- author name-->
                        <div>
                            {{details.author}}
                        </div>
                    </div>
                </div>

                <!-- col -->
                <div class="col-6">
                    <div class="hover-appears">
                        <div>
                            <i class="far fa-clock"></i>
                        </div>
                        <!-- day upload -->
                        <div>
                            2 Days Ago
                        </div>
                    </div>
                </div>

            </div>

            <!-- title -->
            <h6>{{details.title}}</h6>

            <!-- paragrafo -> solo in hover -->
            <div class="hover-appears">
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit.</p>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "CardNews",
    props:{
        details: Object
    }
}
</script>

<style lang="scss">
.card-news-wrapping{
    width: 400px;
    height: 400px;
    position: relative;
    overflow: hidden;
    border-radius: 10px;
    .background-img{
        width: 100%;
        height: 100%;
        overflow: hidden;
        img{
            width: 100%;  
            height: 100%;  
            object-fit: cover;
        }
    }
    .text{
        width: 100%;
        height: 100%;
        background-color: rgba($color: #000000, $alpha: 0.5);
        position: absolute;
        top: 0;
        color: white;
        display: flex;
        flex-direction: column;
        justify-content: end;
        text-align: center;
        padding: 30px 20px;
        .row{
            flex-grow: 1;
            .col-6{
                .hover-appears > div{
                    float: left;
                }
                i{
                    padding: 0px 10px;
                }
            }
        }
        h6{
            font-size: 29px;
            padding: 10px 0;
        }
    }
}

// active
.hover-appears{
    display: none;
}
.card-news-wrapping:hover .hover-appears{
    display: block;
}

</style>