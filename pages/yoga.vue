<template>
  <Layout>
    <div>
      <fullWidth
        class="full-width"
        title="Yoga"
        description="Viens yogater à l'espace Ivy !"
        textcolor="white"
        link=""
        imgsrc="img/yoga/yoga-dan.jpg"
      />
      <textBlock
        class="full-width"
        title="Histoire"
        description="Courte histoire de Dan."
        textcolor="black"
      />
      <div class="container-row">
        <fullWidth
          class="full-width"
          title=""
          description=""
          textcolor=""
          link=""
          imgsrc="img/yoga/yoga-dan-2.jpg"
        />
        <h2 class="section-title">
          Descriptifs de classes
        </h2>
        <div class="demi-width-descriptifs">
          <descriptifs
            title="FLOW FOR ALL"
            description="Entre le Flow Chill (Hatha Flow Yoga) et le Flow Go (Vinyasa Yoga) cette classe est une combinaison de postures statiques (Hatha Yoga) et de mouvements (Vinyasa Yoga). Une pratique pour tous, ou les débutants comme les plus initiés auront du plaisir!"
          />
          <descriptifs
            title="FLOW CHILL"
            description="Ce cours de type Hatha Flow Yoga est une combinaison de postures statiques (Hatha Yoga) et de mouvement (Vinyasa Yoga). Énergisant, il renforce le corps, fait circuler l'énergie et canalise l'esprit. Un cours tous niveaux!"
          />
          <descriptifs
            title="FLOW GO"
            description="Ce cours de type Vinyasa Yoga à un rythme plus soutenu que le Flow Chill (Hatha Flow Yoga) car il inclut des séquences plus stimulantes. Il convient aux pratiquants qui ont une bonne base en yoga!"
          />
          <descriptifs
            title="KICK ASS"
            description="Savant mélange de Vinyasa Yoga et de Fitness, ce cours est parfait pour les gens qui s’entraînent régulièrement ou qui ont une pratique de yoga bien établie. Il est aussi idéal pour toutes personnes motivées souhaitant se remettre en forme rapidement. Cette classe d'un niveau plus exigeant que le Flow Go (Vinyasa Yoga) promet son lot de challenge. Apportez une serviette car vous risquez sérieusement de transpirer!"
          />
          <descriptifs
            title="RELAX"
            description="Délicieux mélange de Yin, Thérapeutique, Restoratif et Nidra Yoga. Excellent pour calmer le mental, gagner en Flexibilité et se Relaxer. Ce cours est parfait pour lâcher prise complètement et pour une totale régénération. Un cours tous niveaux!"
          />
          <descriptifs
            title="UP & DOWN"
            description="2/3 Flow Go (Vinyasa Yoga) & 1/3 Relax (mix de Yin, Therapeutique, Restoratif & Nidra Yoga)! Cette séance est une combinaison parfaite de Vinyasa Yoga (mouvements debout) et de Yin Yoga (postures assises et allongées + relaxation). Un reset complet sur l’heure du midi afin de repartir pleinement revitalise pour le reste de la journée. Un cours tous niveaux qui offre quelques défis!"
          />
          <descriptifs
            title="MOBILITÉ"
            description="Ce cours « carte blanche » est très versatile! Exercices spécifiques d’alignement postural, mouvements fonctionnels, transition entre deux postures. Plusieurs possibilités sont offertes adaptées aux participants. Cours tous niveaux!"
          />
          <descriptifs
            title="YOGA DOUX"
            description="Ce cours de type Hatha Yoga est accessible à tous et convient particulièrement aux personnes qui ont des limitations physiques, que ce soit lié à l’âge, la maladie, une blessure. Une combinaison de mouvements lents et de postures de type Thérapeutique. Excellent pour rester actif tout en douceur!"
          />
        </div>
        <h2 class="section-title">
          Liste de prix
        </h2>
        <div class="demi-width-descriptifs">
          <prices
            title="Intro"
            price="50$"
            description="1er Mois de Yoga Illimité.(Valable 1 fois par personne)"
          />
          <prices
            title="Intro"
            price="50$"
            backcolor="#FCDA1E"
            description="1er Mois de Yoga Illimité.(Valable 1 fois par personne)"
          />
          <prices
            title="Intro"
            price="50$"
            description="1er Mois de Yoga Illimité.(Valable 1 fois par personne)"
          />
        </div>
      </div>
      <fullWidth
        class="full-width"
        title="Espace"
        description="Loue l'espace pour ta prochaine activité!"
        textcolor="black"
        link="location"
        imgsrc="img/studio/photo-loue-espace.jpg"
      />
    </div>
  </Layout>
</template>

<script>
import fullWidth from '~/components/fullWidthBloc.vue'
import textBlock from '~/components/text-block.vue'
import descriptifs from '~/components/descriptifs.vue'
import prices from '~/components/prix.vue'

export default {
  metaInfo: {
    title: 'Yoga'
  },
  components: {
    fullWidth,
    textBlock,
    descriptifs,
    prices
  }
}
</script>
