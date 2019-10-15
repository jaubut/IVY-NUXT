<template>
  <Layout>
    <div>
      <fullWidth
        class="full-width-v-two"
        title="Évènements"
        description="Soit au courant de tous les événements IVY"
        textcolor="black"
        link=""
        imgsrc="img/studio/photo-loue-espace.jpg"
      />
      <div class="full-width-v-two">
        <h2 class="section-title">
          Consulte tous les évènements de l'espace Ivy<br>
          <span><h3>Mise à jour sur <a target="_blank" href="https://www.facebook.com/pg/espaceivy/events/?ref=page_internal">Facebook</a></h3></span>
        </h2>
        <a class="reserve" target="_blank" href="https://www.facebook.com/pg/espaceivy/events/?ref=page_internal">Événements</a>
      </div>
      <h2 class="section-title">
        Exposition en cours<br>
        <span><h3>En savoir plus sur l'artiste: <a target="_blank" href="https://www.facebook.com/pg/espaceivy/events/?ref=page_internal">Dan</a></h3></span>
      </h2>
      <carousel class="full-width-v-two" :per-page="2" :mouse-drag="true">
        <slide class="slideshow">
          <img class="img-galerie" src="~assets/img/studio/photo-loue-espace.jpg" alt="">
        </slide>
        <slide class="slideshow">
          <img class="img-galerie" src="~assets/img/studio/photo-loue-espace.jpg" alt="">
        </slide>
        <slide class="slideshow">
          <img class="img-galerie" src="~assets/img/studio/photo-loue-espace.jpg" alt="">
        </slide>
        <slide class="slideshow">
          <img class="img-galerie" src="~assets/img/studio/photo-loue-espace.jpg" alt="">
        </slide>
      </carousel>
    </div>
  </Layout>
</template>

<script>
import { Carousel, Slide } from 'vue-carousel'
import fullWidth from '~/components/fullWidthBloc.vue'

export default {
  components: {
    fullWidth,
    Carousel,
    Slide
  },
  data () {
    return {
      title: 'Espace IVY - Événements',
      description: 'Créateur de Valeur et de Mouvement l’Espace IVY est une place unique en son genre! Il s’agit à la fois d’un studio de Yoga et d’une galerie d’Art situé dans un grand loft industriel lumineux niché dans l’immeuble Impérial à Granby classé patrimoine culturel du Québec. L’ambiance y est chaleureuse et décontractée ou l’on se plaît à faire du yoga décomplexé sur des mélodies accrocheuses et des rythmes entraînants. La plupart de nos classes sont ouvertes à tous les niveaux. Le studio de Yoga offre une tarification très accessible et marginale puisque aucun abonnement n’est offert. Zéro obligation, pas de prélèvement automatique, tu payes quand tu viens! Que ce soit pour bouger, lâcher prise, croire en toi, ralentir, te sentir plus ancré, plus souple, plus fort ou moins stressé, l’Espace IVY à Granby est une place où se retrouver afin de partager une pratique de Yoga entre amis, collègues ou en famille. Un lieu de rencontre et d’échange qui fait la promotion des Arts par des expositions et des événements. Bonne humeur à volonté et imperfections bienvenues!'
    }
  },
  head () {
    return {
      title: this.title,
      meta: [
        { hid: 'og:image', property: 'og:image', content: '/img/studio/photo-loue-espace.jpg' },
        // hid is used as unique identifier. Do not use `vmid` for it as it will not work
        { hid: 'description', name: 'description', content: this.description }
      ]
    }
  }
}
</script>

<style scoped>
.container-facebook {
  display: flex;
  justify-content: center;
  align-items: center;
}
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
.img-galerie {
  height: auto;
  max-width: 45vw;
}
.slideshow {
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0.75rem;
}
</style>
