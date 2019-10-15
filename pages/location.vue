<template>
  <Layout>
    <div>
      <fullWidth
        class="full-width-v-two"
        title="l'espace Ivy"
        description="Loue l'espace pour ta prochaine activité!"
        textcolor="white"
        link=""
        imgsrc="img/studio/photo-loue-espace.jpg"
      />
      <photos
        imgsrcun="img/studio/photo-cours-dan.jpg"
        imgsrcdeux="img/studio/vestiere.jpg"
        imgsrctrois="img/studio/bureau.jpg"
        imgsrcquatre="img/studio/salle-essayage.jpg"
        imgsrccinq="img/studio/eau.jpg"
      />
      <div class="container-row">
        <fullWidth
          class="demi-width-v-two"
          imgsrc="img/studio/galerie.jpg"
        />
        <textBlock
          class="demi-width-v-two"
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
          :descriptionlist="materiels"
        />
        <descriptifs
          title="Équipement"
          :descriptionlist="equipements"
        />
      </div>
      <h2 class="section-title">
        Liste de prix <span class="taxes">+Tx</span>
      </h2>
      <div class="container-prix">
        <prices
          class="prices-v-two"
          title="1H"
          price="35$"
          description=""
          cta="Réserve"
        />
        <prices
          class="prices-v-two"
          title="Bloc de 4H"
          price="120$"
          backcolor=""
          bordercolor="white"
          description=""
          cta="Réserve"
        />
        <prices
          class="prices-v-two"
          title="Bloc de 8H"
          price="250$"
          description=""
          cta="Réserve"
        />
      </div>
    </div>
  </Layout>
</template>

<script>
import fullWidth from '~/components/fullWidthBloc.vue'
import textBlock from '~/components/text-block.vue'
import descriptifs from '~/components/descriptifs.vue'
import prices from '~/components/prixReserve.vue'
import photos from '~/components/blocphoto.vue'

export default {
  components: {
    fullWidth,
    textBlock,
    prices,
    descriptifs,
    photos
  },
  data () {
    return {
      materiels: ['40 Blocs de liège', '25 Traversins Moyen en coton', '25 Sangles en coton', '20 Yoga Tune Up', 'Therapy Balls', '20 Chaises pliantes', '10 Tapis BMAT', '25 Couvertures cotton indien'],
      equipements: ['Coin lounge minimaliste & ethnique', 'Coin réception épuré & ergonomique', 'Fontaine Ovopur', 'Access à internet', 'Vidéoprojecteur', 'Speaker Bose Revolve (son à 360 degrés)']
    }
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
@media screen and (max-width: 600px) {
  .taxes {
    font-size: small;
  }
}
</style>
