<template>
  <div id="app">
    <header-container/>
    <main-container :options="options"/>
    <results-container :results="results"/>
    <performance-box/>
    <trainers-container :trainers="trainers"/>
    <news-container :articles="articles"/>
    <footer-box/>
  </div>
</template>

<script>
import HeaderContainer from './components/HeaderContainer.vue'
import MainContainer from './components/MainContainer.vue'
import FooterBox from './components/FooterBox.vue'
import ResultsContainer from './components/ResultsContainer.vue'
import PerformanceBox from './components/PerformanceBox.vue'
import TrainersContainer from './components/TrainersContainer.vue'
import NewsContainer from './components/NewsContainer.vue'


export default {
  name: 'App',
  components: {
    HeaderContainer,
    MainContainer,
    FooterBox,
    ResultsContainer,
    PerformanceBox,
    TrainersContainer, 
    NewsContainer
  },

  data() {
    return {

      options: [
        {
          img: '',
          activity: 'Streng & Conditioning',
          description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Obcaecati sequi commodi veritatis facilis pariatur ad',
        },
        {
          img: '',
          activity: 'Fitness & Cardio',
          description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Obcaecati sequi commodi veritatis facilis pariatur ad',
        },
        {
          img: '',
          activity: 'Flexibility & Rest',
          description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Obcaecati sequi commodi veritatis facilis pariatur ad',
        },
        {
          img: '',
          activity: 'Health & Diet',
          description: 'Lorem ipsum dolor sit, amet consectetur adipisicing elit. Obcaecati sequi commodi veritatis facilis pariatur ad',
        },
      ],
      
      results: [
        {
          image: 'review_1-compressor.jpg',
          name: "Tara Smith",
          review: "The trainers at Avada Gym have helped me reach my fitness goals beyond anything I could of hoped for. I love it!", 
        },
        {
          mage: 'review_3-compressor-2.jpg',
          name: 'Simon Chel',
          review: 'The atmosphere at Avada Gym is amazing, the people are even better. All in all, it is a great place to work out.',
        },
        {
          mage: 'review_2-compressor.jpg',
          name: 'Jen Wirth',
          review: 'The facilities at Avada Gym stood out to me the most. They are well maintained and have high quality equipment',
        },
        {
          mage: 'review_4-compressor-2.jpg',
          name: 'Jeff Glum',
          review: 'No bad things to say abut Avada Gym, they are top notch at every corner and truly take care of their customers.',
        },
      ],

      trainers: [
        {
          photo: 'trainer1.jpg',
          name: 'Ann Baker',
          role: 'Personal Trainer',
          description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. A rerum nihil obcaecati ipsum',
        },
        {
          photo: 'trainer3.jpg',
          name: 'Anne Warren',
          role: 'Personal Trainer',
          description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. A rerum nihil obcaecati ipsum',
        },
        {
          photo: 'trainer4.jpg',
          name: 'Peter Rice',
          role: 'Personal Trainer',
          description: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. A rerum nihil obcaecati ipsum',
        },
      ], 

      articles: [
        {
          img: 'blog1.jpg',
          title: 'Train with free weights or your body weight?',
          anteprima: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec pretium, tortor vitae porttiror suscipit, sapien purus aliquet risus.',
        },
        {
          img: 'blog6.jpg',
          title: 'Nutritional advice that will keep you training',
          anteprima: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec pretium, tortor vitae porttiror suscipit, sapien purus aliquet risus.',
        },
        {
          img: 'trainer4.jpg',
          title: 'Simple principles for you next workout',
          anteprima: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec pretium, tortor vitae porttiror suscipit, sapien purus aliquet risus.',
        },
        {
          img: 'blog4.jpg',
          title: 'To be number one, train like you are number two',
          anteprima: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec pretium, tortor vitae porttiror suscipit, sapien purus aliquet risus.',
        },
        {
          img: 'trainer3.jpg',
          title: 'Top 5 mistakes every gym member makes',
          anteprima: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec pretium, tortor vitae porttiror suscipit, sapien purus aliquet risus.',
        },
        {
          img: 'trainer1.jpg',
          title: 'The myths of shedding body fat explored',
          anteprima: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec pretium, tortor vitae porttiror suscipit, sapien purus aliquet risus.',
        },
      ]
    }
  }
}
</script>

<style ,
    NewsContainerlang="scss">
@import './style/body.scss';
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;500&display=swap');
</style>