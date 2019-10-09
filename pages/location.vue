<template>
  <Layout>
    <div>
      <fullWidth
        class="full-width"
        title="l'espace Ivy"
        description="Loue l'espace pour ta prochaine activité!"
        textcolor="white"
        link=""
        imgsrc="img/studio/photo-loue-espace.jpg"
      />
      <div class="full-width-photos">
        <img class="portrait-photo photo" src="~/assets/img/studio/photo-cours-dan.jpg" alt="">
        <img class="landscape-photo photo" src="~/assets/img/studio/galerie.jpg" alt="">
        <img class="landscape-photo photo" src="~/assets/img/studio/salle-essayage.jpg" alt="">
        <img class="portrait-photo photo" src="~/assets/img/studio/vestiere.jpg" alt="">
      </div>
      <div class="container-row">
        <fullWidth
          class="demi-width"
          title=""
          description=""
          textcolor="white"
          link=""
          imgsrc="img/yoga/yoga-dan-2.jpg"
        />
        <textBlock
          class="demi-width"
          title="Informations"
          description="Grand loft industriel lumineux classé patrimoine culturel du Québec! Capacité d’accueil de 30 personnes (pour le yoga) 1550 Pi2 / 15Pi de hauteur sous plafond. Plancher de bois franc."
          textcolor="black"
        />
      </div>
      <h2 class="section-title">
        Inclusions
      </h2>
      <div class="demi-width-descriptifs">
        <descriptifs
          title="Matériel"
          description="40 Blocs de liège - 25 Traversins Moyen en coton / 25 Sangles en coton / 20 Yoga Tune Up – Therapy Balls / 20 Chaises pliantes / 10 Tapis BMAT/ 25 Couvertures cotton indien."
        />
        <descriptifs
          title="Équipement"
          description="Coin lounge minimaliste & ethnique / Coin réception épuré & ergonomique / Fontaine Ovopur / Access à internet / Vidéoprojecteur / Speaker Bose Revolve (son à 360 degrés)."
        />
      </div>
      <h2 class="section-title">
        Liste de prix <span class="taxes">+Tx</span>
      </h2>
      <div class="demi-width-descriptifs">
        <prices
          title="1H"
          price="35$"
          description=""
        />
        <prices
          title="Bloc de 4H"
          price="120$"
          backcolor="#FCDA1E"
          description=""
        />
        <prices
          title="Bloc de 8H"
          price="250$"
          description=""
        />
      </div>
    </div>
  </Layout>
</template>

<script>
import fullWidth from '~/components/fullWidthBloc.vue'
import textBlock from '~/components/text-block.vue'
import descriptifs from '~/components/descriptifs.vue'
import prices from '~/components/prix.vue'

export default {
  components: {
    fullWidth,
    textBlock,
    prices,
    descriptifs
  }
}
</script>

<style scoped>
.landscape-photo {
  height: auto;
  width: 50%;
}
.portrait-photo {
  height: auto;
  max-width: 40%;
}
.taxes {
  font-size: 2rem;
}
</style>
