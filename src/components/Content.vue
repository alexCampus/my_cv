<template>
    <div class="content">
      <transition
        enter-active-class="animated fadeInLeft"

      >
        <Resume v-if="clickFromNav === 'resume'" @redirect="redirectFromResume"></Resume>
      </transition>
      <transition
        enter-active-class="animated fadeInLeft"

      >
        <Skills v-if="clickFromNav === 'skills'"></Skills>
      </transition>
      <transition
        enter-active-class="animated fadeInLeft"

      >
        <Portfolio v-if="clickFromNav === 'portfolio'"></Portfolio>
      </transition>
      <transition
        enter-active-class="animated fadeInLeft"

      >
        <Contact v-if="clickFromNav === 'contact'"></Contact>
      </transition>
    </div>
</template>

<script>
    import profilImage from './profilImage'
    import Resume from './Content/Resume'
    import Portfolio from './Content/Portfolio'
    import Skills from './Content/Skills'
    import Contact from './Content/Contact'
    export default {
  name: 'Content',
      props: ['clickFromNav'],
      components: {Contact, Skills, Portfolio, Resume, profilImage},
      data () {
        return {
          isVisible: false
        }
      },
      methods: {
        redirectFromResume: function (value) {
          this.clickFromNav = (value === 'contact') ? 'contact' : this.clickFromNav
        }
      }
    }
</script>

<style scoped>
  .content {
    margin-left: 1%;
    width: 45%;
    min-width: 45%;
    background-color: #f0f0f0;
    overflow-y: scroll;
    max-height: 580px;
  }
</style>
