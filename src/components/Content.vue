<template>
    <div class="content">
      <Resume v-if="clickFromNav === 'resume'"></Resume>
      <Skills v-if="clickFromNav === 'skills'"></Skills>
      <Portfolio v-if="clickFromNav === 'portfolio'"></Portfolio>
      <Contact v-if="clickFromNav === 'contact'"></Contact>
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
      props: ['clickFromNav', 'isVisible'],
      components: {Contact, Skills, Portfolio, Resume, profilImage}
    }
</script>

<style scoped>
  .backgroundColor {
    background-color: #08aeac;
    color:#fff;
  }
  .backgroundColor a {
    color:#fff;
  }
  .backgroundColor a:hover {
    color: #084f4d;
  }
  .color {
    color: #08aeac;
  }
  .bold {
    font-weight:bold;
    letter-spacing: -3px;
  }
  .semiBold {
    font-weight:400;
  }
.content {
  margin-left: 1%;
  width: 65%;
  background-color: #f0f0f0;
}
.socialIcons {
  margin-top: 3%;
  margin-bottom: 5%;
}

.socialIcons a:hover {
  background-color: #08aeac;
}

hr {
  height: 30px;
  border-style: solid;
  border-color: #8c8b8b;
  border-width: 1px 0 0 0;
  border-radius: 20px;
  max-width: 90%;
  opacity: 0.4;
}
hr:before {
  display: block;
  content: "";
  height: 30px;
  margin-top: -31px;
  border-style: solid;
  border-color: #8c8b8b;
  border-width: 0 0 1px 0;
  border-radius: 20px;
}
  .alert {
    width: 85%;
    margin: auto;
  }

</style>
