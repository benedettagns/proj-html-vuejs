<template>
    <header>
        <div class="menu-container">

            <img src="../assets/gym_logo_1x.png" alt="">

            <ul>
                <li>home</li>
                <li>about us</li>
                <li>facilities</li>
                <li>membership</li>
                <li>testimonials</li>
                <li>blog</li>
            </ul>
        </div>

        <div class="title-container">

            <h1>no pain no gain</h1>

            <p>Motivation is what gets ypu started. Habit is what keeps you going.</p>

            <button>JOIN US TODAY</button>
        </div>
        
    </header>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
header {
    background: url('../assets/home-banner.jpg') no-repeat;
    background-size: cover;
    height: 100vh;

    .menu-container {
        display: flex;
        justify-content: space-between;
        align-items: center;

        img {
            width: 150px;
            margin-top: 50px;
            margin-left: 30px ;
        }

        ul {
            color: white; 
            list-style: none;
            display: flex;
            text-transform: uppercase;
            margin-top: 50px;
            margin-right: 30px;

            li {
                padding: 10px;

                &:hover {
                cursor: pointer;
                color: #d5625f;
                }
            }
        }
    }

    .title-container {
        text-align: center;
        margin-top: 150px;
        line-height: 50px;

        h1 {
            font-size: 70px;
            color: white;
            text-transform: uppercase;
        }

        p {
            color: grey;
            font-size: 16px;
        }

        button {
            height: 40px;
            width: 150px;
            background-color: rgba(0, 0, 0, 0);
            color: grey;

        }
    }
}
</style>