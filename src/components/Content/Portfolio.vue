<template>
    <b-container class="margin">
      <h2 class="bold text-left">Portfolio</h2>
      <hr class="hr">
      <div class="imgCard">
        <b-card title="Le Labo Bois"
                img-src="../../static/lelabobois.png"
                img-alt="Image"
                img-bottom>
          <p class="card-text">
            Site One Page en Laravel 5.3 et VueJS 2.0 <em>(Conception & réalisation)</em>
          </p>
          <b-button href="http://www.lelabobois.fr" target="_blank" variant="info">Voir le site</b-button>
        </b-card>
      </div>

      <div class="imgCard">
        <b-card title="La Banda Tujumi"
                img-src="../../static/tujumi.jpg"
                img-alt="Image"
                img-bottom>
          <p class="card-text">
            Site en Laravel 5.3 avec interface admin, réservation et inscription <em>(Conception & réalisation)</em>
          </p>
          <b-button href="https://www.banda-tujumi.fr" target="_blank" variant="info">Voir le site</b-button>
        </b-card>
      </div>

      <div class="imgCard">
        <b-card title="Achat Ville"
                img-src="../../static/achatVille.jpg"
                img-alt="Image"
                img-bottom>
          <p class="card-text">
            Site en PHP 7.0, Mysql, Js ... <em>(Support, Maintenance & Evolution)</em>
          </p>
          <b-button href="https://www.achat-ville.com/" target="_blank" variant="info">Voir le site</b-button>
        </b-card>
      </div>

      <div class="imgCard">
        <b-card title="Boutiques Solo"
                img-src="../../static/logoEolas.png"
                img-alt="Image"
                img-bottom>
          <p class="card-text">
            Site en PHP 7.0, Mysql, Js ... <em>(Support, Maintenance & Evolution)</em>
          </p>
          <b-button href="https://www.miss-pieces.com/" target="_blank" variant="info">Exemple de site</b-button>
          <b-button href="https://www.croque-montagne.fr" target="_blank" variant="info">Exemple de site</b-button>
        </b-card>
      </div>
    </b-container>
</template>
<script>
    export default {
  name: 'Portfolio'
    }
</script>

<style scoped>
  .margin {
    margin-top: 5%;
    margin-bottom: 5%;
  }
  .bold {
    font-weight: 400;
  }
  .hr {
    border: 0;
    height: 1px;
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.75), rgba(0, 0, 0, 0));
  }
  .imgCard {
    margin-top: 5%;
  }
</style>
