<template lang="">
    <div class="content">
        <div class="slides">
            <input type="radio" name="slide" id="slide1" checked>
            <input type="radio" name="slide" id="slide2">
            <input type="radio" name="slide" id="slide3">
            <input type="radio" name="slide" id="slide4">
            <input type="radio" name="slide" id="slide5">

            <div class="slide s1">
                <img src="../../public/1.jpg" alt="godofwar">
            </div>
            <div class="slide">
                <img src="../../public/cadastro.jpg" alt="cadastro">
            </div>
            <div class="slide">
                <img src="../../public/Stray.jpg" alt="stray">
            </div>
            <div class="slide">
                <img src="../../public/farcry6.jpg" alt="farcry6">
            </div>
            <div class="slide">
                <img src="../../public/finalfantasy.jpg" alt="farcry6">
            </div>
        </div>
        <div class="navigation">
            <label class="bar" for="slide1"></label>
            <label class="bar" for="slide2"></label>
            <label class="bar" for="slide3"></label>
            <label class="bar" for="slide4"></label>
            <label class="bar" for="slide5"></label>
        </div>
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>

img{
    width: 90vw;
}
.content{ 
    margin-top: 20px;
    width: 90vw;
    height:  40vh;
    background: linear-gradient(72deg, #3debb0 1%, #8956f3 99%);
    border-radius: 20px;
    overflow: hidden;
    position: relative;
}

.navigation {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translate(-50%);
    display: flex;
}

.bar {
    width: 70px;
    height: 17px;
    border: 2px solid #fff;
    margin: 6px;
    border-radius: 5px;
    cursor: pointer;
    transition: .4s;
}


input{
    display: none;
}

.slides{
    display: flex;
    width: 500%;
    height: 100%;
}

.slide {
    width: 20%;
    transition: .6s;
}

div {
    display: flex;
}

#slide1:checked ~ .s1 {
    margin-left: 0;
}
#slide2:checked ~ .s1 {
    margin-left: -20%;
}
#slide3:checked ~ .s1 {
    margin-left: -40%;
}
#slide4:checked ~ .s1 {
    margin-left: -60%;
}
#slide5:checked ~ .s1 {
    margin-left: -80%;
}

@media (min-width:1200px) {
    .content{ 
        width: 60vw;
        height:  45vh;
    }
}
@media (min-width:1500px) {
    .content{ 
        max-width: 65vw;
        height:  50vh;
    }
}

</style>