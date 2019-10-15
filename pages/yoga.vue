<template>
  <Layout>
    <div>
      <fullWidth
        class="full-width-v-two"
        title="Ivy Yoga"
        description="Viens yogater à l'espace Ivy !"
        textcolor="white"
        link=""
        imgsrc="img/yoga/yoga-dan.jpg"
      />
      <div class="container-row">
        <fullWidth
          class="demi-width-v-two"
          title=""
          description=""
          textcolor="white"
          link=""
          imgsrc="img/yoga/yoga-dan-2.jpg"
        />
        <textBlock
          class="demi-width-v-two"
          title="Notre vision"
          description="Que ce soit pour bouger, lâcher prise, croire en toi, ralentir, te sentir plus ancré, plus souple, plus fort ou moins stressé, l’Espace IVY à Granby est une place où se retrouver afin de partager une pratique de Yoga entre amis, collègues ou en famille. Un lieu de rencontre et d’échange qui fait la promotion des Arts par des expositions et des événements."
          textcolor="black"
        />
      </div>
      <h2 class="section-title">
        Description des classes
      </h2>
      <div class="demi-width-descriptifs">
        <descriptifs
          title="FLOW FOR ALL"
          description="Entre le Flow Chill (Hatha Flow Yoga) et le Flow Go (Vinyasa Yoga) cette classe est une combinaison de postures statiques (Hatha Yoga) et de mouvements (Vinyasa Yoga). Une pratique pour tous, ou les débutants comme les plus initiés auront du plaisir!"
          logoname="liere-debout"
        />
        <descriptifs
          title="FLOW CHILL"
          description="Ce cours de type Hatha Flow Yoga est une combinaison de postures statiques (Hatha Yoga) et de mouvement (Vinyasa Yoga). Énergisant, il renforce le corps, fait circuler l'énergie et canalise l'esprit. Un cours tous niveaux!"
          logoname="liere"
        />
        <descriptifs
          title="FLOW GO"
          description="Ce cours de type Vinyasa Yoga à un rythme plus soutenu que le Flow Chill (Hatha Flow Yoga) car il inclut des séquences plus stimulantes. Il convient aux pratiquants qui ont une bonne base en yoga!"
          logoname="moudra"
        />
        <descriptifs
          title="KICK ASS"
          description="Savant mélange de Vinyasa Yoga et de Fitness, ce cours est parfait pour les gens qui s’entraînent régulièrement ou qui ont une pratique de yoga bien établie. Il est aussi idéal pour toutes personnes motivées souhaitant se remettre en forme rapidement. Cette classe d'un niveau plus exigeant que le Flow Go (Vinyasa Yoga) promet son lot de challenge. Apportez une serviette car vous risquez sérieusement de transpirer!"
          logoname="pigeon"
        />
        <descriptifs
          title="RELAX"
          description="Délicieux mélange de Yin, Thérapeutique, Restoratif et Nidra Yoga. Excellent pour calmer le mental, gagner en Flexibilité et se Relaxer. Ce cours est parfait pour lâcher prise complètement et pour une totale régénération. Un cours tous niveaux!"
          logoname="serpent"
        />
        <descriptifs
          title="UP & DOWN"
          description="2/3 Flow Go (Vinyasa Yoga) & 1/3 Relax (mix de Yin, Therapeutique, Restoratif & Nidra Yoga)! Cette séance est une combinaison parfaite de Vinyasa Yoga (mouvements debout) et de Yin Yoga (postures assises et allongées + relaxation). Un reset complet sur l’heure du midi afin de repartir pleinement revitalise pour le reste de la journée. Un cours tous niveaux qui offre quelques défis!"
          logoname="logo-footer"
        />
        <descriptifs
          title="MOBILITÉ"
          description="Ce cours « carte blanche » est très versatile! Exercices spécifiques d’alignement postural, mouvements fonctionnels, transition entre deux postures. Plusieurs possibilités sont offertes adaptées aux participants. Cours tous niveaux!"
          logoname="logo-menu"
        />
        <descriptifs
          title="YOGA DOUX"
          description="Ce cours de type Hatha Yoga est accessible à tous et convient particulièrement aux personnes qui ont des limitations physiques, que ce soit lié à l’âge, la maladie, une blessure. Une combinaison de mouvements lents et de postures de type Thérapeutique. Excellent pour rester actif tout en douceur!"
          logoname="lion"
        />
      </div>
      <h2 class="section-title">
        Liste de prix
      </h2>
      <div class="container-prix">
        <prices
          class="prices-v-two"
          title="Intro"
          price="50$"
          backcolor=""
          bordercolor="white"
          description="1er Mois de Yoga Illimité (Valable 1 fois par personne)"
        />
        <prices
          class="prices-v-two"
          title="1 Semaine Illimité"
          price="35$"
          description="Aucun engagement, tu payes à la semaine"
        />
        <prices
          class="prices-v-two"
          title="1 Mois Illimité"
          price="80$"
          description="Aucun engagement, tu payes au mois."
        />
        <prices
          class="prices-v-two"
          title="3 Mois Illimité"
          price="210$"
          description="Aucun engagement, tu payes une fois au 3 mois."
        />
        <prices
          class="prices-v-three"
          title="Drop-in"
          price="15$"
          description="Classe à la carte"
          bordercolor="white"
        />
        <prices
          class="prices-v-three"
          title="20 Classes"
          price="240$"
          description="- 20% ( = 12 $/Cours) - Valide 12 mois"
        />
        <prices
          class="prices-v-three"
          title="10 Classes"
          price="135$"
          description="- 10% ( = 13.5 $/Cours) - Valide 6 mois"
        />
      </div>
      <div class="full-width-v-two">
        <h2 class="section-title">
          Réserve ta classe sur <a target="_blank" href="https://mindbody.io/fitness/studios/ivy-espace-yoga-arts-communaute">Mindbody</a>
        </h2>
        <a class="reserve" target="_blank" href="https://mindbody.io/fitness/studios/ivy-espace-yoga-arts-communaute">Réserve ta classe</a>
      </div>
      <h2 class="section-title">
        Horaire du 2 septembre au 21 decembre <br>
        <span><h3>Mise à jour sur <a target="_blank" href="https://mindbody.io/fitness/studios/ivy-espace-yoga-arts-communaute">Mindbody</a>. Sujet à changement sans préavis.</h3></span>
      </h2>
      <div class="container-column">
        <img class="image" src="~/assets/img/horaire/horaire-web.png" alt="">
      </div>
      <client-only placeholder="Loading...">
        <div class="container-column">
          <healcode-widget data-type="schedules" data-widget-partner="object" data-widget-id="bd11501717a9" data-widget-version="1" />
        </div>
      </client-only>
    </div>
  </Layout>
</template>

<script>
import ClientOnly from 'vue-client-only'
import fullWidth from '~/components/fullWidthBloc.vue'
import textBlock from '~/components/text-block.vue'
import descriptifs from '~/components/descriptifs.vue'
import prices from '~/components/prix.vue'

export default {
  metaInfo: {
    title: 'Yoga'
  },
  components: {
    ClientOnly,
    fullWidth,
    textBlock,
    descriptifs,
    prices
  }
}
</script>

<style scoped>
.reserve {
  display: flex;
  justify-content: center;
  align-items: center;
  border: none;
  color: black;
  background-color: #FCDA1E;
  width: 10rem;
  height: 3rem;
  border-radius: 5px;
  box-shadow: 1px 2px rgba(0, 0, 0, 0.1);
}
</style>
