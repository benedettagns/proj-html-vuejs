<template>
    <div class="results-container">
        <h1>REAL WORLD RESULTS</h1>
        <img src="../assets/divider-xx-red.png" alt="">

        <div class="box-container"> 
            <div class="box-utenti" v-for="(result, index) in results" :key="index">
                <div>
                    <img :src="result.image" alt="">
                </div>
                <div>
                    <p>{{result.review}}</p>
                    <span>- {{result.name}}</span>
                </div>    
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        results: Array
    }  
    
}
</script>

<style lang="scss" scoped>
.results-container {
    background-color: #252a2d;
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