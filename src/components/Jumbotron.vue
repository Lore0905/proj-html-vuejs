<template>
    <div class="wrapping">
        <div id="jumbotron-img">
            <img src="../assets/hero-image.png" alt="">
        </div>
        <div id="jumbotron-text">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Suscipit nisi cum optio quasi ea praesentium sapiente est laudantium commodi quidem. Corporis aspernatur iste maiores. Minima iste quis repellat ea aliquid!
        </div>
    </div>
</template>

<script>
export default {
    name: "jumbotron"
}
</script>

<style lang="scss">
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
    }

}

</style>