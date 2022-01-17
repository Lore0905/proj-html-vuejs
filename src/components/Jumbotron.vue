<template>
    <div class="wrapping">
        <div id="jumbotron-img">
            <img src="../assets/hero-image.png" alt="banner">
        </div>
        <div id="jumbotron-text">
            <h1>Lead<span id="tilde">~</span>Customer</h1>

            <p>Successful strategies require data analysis, creativity and customer focus, taking advantage of the latest technologies to offer excellent services</p>
            <!-- buttons -->
            <div class="btn first-btn">
                <button>GET IN TOUCH</button>
            </div>
            <div class="btn second-btn">
                <button>READ MORE</button>
            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: "jumbotron"
}
</script>

<style lang="scss">
@import '../style/variables.scss';
.wrapping{
    width: 100%;
    height: 80vh;
    position: relative;
    
    #jumbotron-img{
        width: 100%;
        height: 100%;
        overflow: hidden;
        object-position: bottom;
        
        img{
            width: 100%;  
            height: 100%;  
            object-fit: cover;
            object-position: center;  
        }
    }

    #jumbotron-text{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
        color: white;

        h1{
            font-weight: 900;
            font-size: 70px;
            display: flex;
            align-items: center;
            justify-content: center;
            #tilde{
                font-size: 110px;
            }
        }
        p{
            font-size: 22px;
            color: $grey;
            padding-bottom: 20px;
        }
    }
}
// background black banner
.wrapping::before{
    content: "";
    background-color: rgba(0, 0, 0, 0.7);
    width: 100%;
    height: 100%;
    position: absolute;
    top: 0px;
}

</style>