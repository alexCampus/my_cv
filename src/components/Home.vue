<template>
    <div class="home">
      <profilImage></profilImage>
      <h1 class="bold">Hi, i'm <br><span class="color">Alexandre De Pembroke</span></h1>
      <h5 class="semiBold">Fullstack Web Developer</h5>
     <hr>
      <p>Bellicis efferebantur fames efferebantur quam incohibili saeviore legiones quam tresque efferebantur desperatio bellicis Castricius comes matris
        matris efferebantur legiones Castricius matris quam saeviore quam Castricius incohibili viribus excidium viribus rabie.</p>
      <b-alert show class="alert backgroundColor">E-Mail: <a href="mailto:alex.depem@hotmail.fr">alex.depem@hotmail.fr</a> / Phone <a href="tel:+33626254358">+33 6 26 25 43 58</a></b-alert>
      <div class="socialIcons">
        <b-button target="_blank" href="https://www.linkedin.com/in/de-pembroke-alexandre/"><i class="fab fa-linkedin-in"></i></b-button>
        <b-button target="_blank" href="https://github.com/alexCampus"><i class="fab fa-github"></i></b-button>
      </div>
    </div>
</template>

<script>
    import profilImage from './profilImage'
    export default {
  name: 'Home',
      components: {profilImage}
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
.home {
  /*width: 65%;*/
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
