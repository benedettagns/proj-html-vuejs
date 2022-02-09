<template>
    <div class="results-container">
        <h1>REAL WORLD RESULTS</h1>
        <img src="../assets/divider-xx-red.png" alt="">

        <div class="box-container"> 
            <div class="box-utenti">
                <div>
                    <img src="../assets/review_1-compressor.jpg" alt="">
                </div>
                <div>
                    <p>"The trainers at Avada Gym have helped me reach my fitness goals beyond anything I could of hoped for. I love it!"</p>
                    <span>- Tara Smith</span>
                </div>    
            </div>

            <div class="box-utenti">
                <div>
                    <img src="../assets/review_3-compressor-2.jpg" alt="">
                </div>
                <div>
                    <p>"The atmosphere at Avada Gym is amazing, the people are even better. All in all, it is a great place to work out."</p>
                    <span>- Simon Chel</span>
                </div>    
            </div>

            <div class="box-utenti">
                <div>
                    <img src="../assets/review_2-compressor.jpg" alt="">
                </div>
                <div>
                    <p>"The facilities at Avada Gym stood out to me the most. They are well maintained and have high quality equipment"</p>
                    <span>- Jen Wirth</span>
                </div> 
            </div>

            <div class="box-utenti">
                <div>
                    <img src="../assets/review_4-compressor-2.jpg" alt="">
                </div>
                <div>
                    <p>"No bad things to say abut Avada Gym, they are top notch at every corner and truly take care of their customers."</p>
                    <span>- Jeff Glum</span>
                </div>   
            </div>


        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.results-container {
    background-color: rgb(41, 40, 40);
    text-align: center;
    
    h1 {
        color: white; 
        padding-top: 50px;
        padding-bottom: 20px;
    }

    .box-container {
        width: 900px;
        display: flex;
        flex-wrap: wrap;
        margin: 0 auto;

        .box-utenti {
            background-color: rgba(0, 0, 0, 0.4);
            display: flex;
            width: 400px;
            height: 150px;
            margin: 20px;
            
            p {
                color: white;
                margin-top: 30px;
                margin-left:10px;
                font-size: 12px;
            }

            img {
                width: 100px;
                height: 100px;
                padding: 20px 0 0 10px;
            }

            span {
                color: white;
                font-size: 12px;
            }
        }
    }
}
</style>