<template>
    <div>
        <div class="jumbotron">
            <div class="jumbo-text">
                <p>"I fear not the man who has practiced 10,000 kicks once, but I fear the man who has practiced one kick 10,000 times."</p>
                <img src="../assets/divider-white-xx.png" alt="">
                <p>BRUCE LEE QUOTE OF THE DAY</p>
            </div>    
        </div>

        <div class="trainers-container">
            <h1>MEET OUR TRAINERS</h1>
            <img src="../assets/divider-xx-red.png" alt="">

            <div class="card-container"> 
                <div class="card" v-for="(trainer, index) in trainers" :key="index">
                    <img :src="trainer.photo" alt="">
                    <p>{{trainer.name}}</p>
                    <p class="job">{{trainer.role}}</p>
                    <p>{{trainer.description}}</p>

                    <div class="social-box">
                        <img src="../assets/instagram.png" alt="">
                    </div>
                </div>
            </div>

            <button>View All Trainers</button>
        </div>   

        
    </div>
</template>

<script>
export default {
    props: {
        trainers: Array
    }
}
</script>

<style lang="scss" scoped>
@import '../style/trainers-container.scss'
</style>