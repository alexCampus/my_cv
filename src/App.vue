<template>
  <div id="app">
    <NavBar @clicked="onClickChild"></NavBar>
    <home></home>
    <transition
      enter-active-class="animated zoomInLeft"
      leave-active-class="animated zoomOutLeft"
    >
      <Content :clickFromNav="dataFromNav" v-if="contentIsVisible"></Content>
    </transition>
  </div>
</template>

<script>
import NavBar from './components/NavBar'
import Home from './components/Home'
import Content from './components/Content'
export default {
  name: 'app',
  components: {
    Content,
    Home,
    NavBar
  },
  data () {
    return {
      dataFromNav: '',
      contentIsVisible: false
    }
  },
  methods: {
    onClickChild: function (value) {
      if (value !== 'home') {
        // document.getElementById('app').style.width = '65%'
        this.contentIsVisible = true
      } else {
        this.contentIsVisible = false
        // document.getElementById('app').style.width = '45%'
      }
      this.dataFromNav = value
    }
  }
}
</script>

<style>
  @import url('https://fonts.googleapis.com/css?family=Montserrat:400,700');
  body {
    font-family: 'Montserrat', sans-serif;
    background-image: url("./assets/back.jpg");
    display: flex;
    justify-content: center;

  }
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 15%;
  max-width: 100%;
  width: 65%;
  display:inline-flex;
}
</style>
