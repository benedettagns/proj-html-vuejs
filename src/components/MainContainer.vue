<template>
    <div>
        <div class="grey-box">
            <div class="divider-container">
                <h1>WORLD CLASS Fitness</h1>
                <img src="../assets/divider-xx-red.png" alt="">
                <p>At Avada Gym, everything we do from top to bottom is of the highest quality to ensure we're equipped 
                    to help you reach your goals of a healthy and fit lifestyle</p>
            </div>
        </div>
        
        <div class="dark-grey-box">
            <div class="sign-up-box">
                <div>
                    <img src="../assets/home_img-compressor.jpg" alt="">
                </div>
                
                <div class="input-box">
                    <h4>Sign Up For A Free Training Season!</h4>
                    <p>Name</p>
                    <input type="text">
                    <p>Email</p>
                    <input type="text">
                    <button>START NOW!</button>
                </div>
            </div>
        </div>

        <div class="jumbotron">
            <div class="jumbo-box">
                <div class="card" v-for="(option, index) in options" :key="index">
                    <!-- <img src="" alt=""> -->
                    <p class="option">{{option.activity}}</p>
                    <img src="../assets/divider-x-red.png" alt="">
                    <p>{{option.description}}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        options: Array
    }
}
</script>

<style lang="scss" scoped>
@import '../style/main-container.scss'
</style>