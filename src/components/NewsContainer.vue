<template>
    <div class="container">
        <h1>PERFORMANCE NEWS</h1>
        <img src="../assets/divider-xx-red.png" alt="">

        <div class="news-container">
            <div class="article-box" v-for="(article, index) in articles" :key="index">
                <img :src="`../assets/${article.img}`" alt="">
                <p> {{article.title}} </p>
                <p> {{article.anteprima}} </p>
            </div>    
        </div>

        <button>READ ALL ARTICLE</button>
    </div>
</template>

<script>
export default {
    props: {
        articles: Array
    }
}
</script>

<style lang="scss" scoped>
.container  {
    display: flex;
    flex-direction: column;
    background-color: #252a2d;
    
    h1{
        color:white;
        padding-top: 40px;
        padding-bottom: 30px;
        margin: 0 auto;
    }

    img {
        padding-bottom: 30px;
        width: 40px;
        margin: 0 auto;
    }

    .news-container {
        width: 1000px;
        margin: 0 auto;
        display: flex;
        flex-wrap: wrap;

        .article-box {
            width: 300px;
            height: 300px;
            margin: 5px;
            background-color: #212425;

            p {
                color: white;
                font-size: 12px;
                padding-left: 20px;
            }
        }
    }

    button {
        width: 200px;
        height: 50px;
        background-color: rgba(37, 37, 37, 0.5);
        color: white;
        text-align: center;
        margin: 20px auto;
    }
}
</style>