<template>
  <Layout>
    <div class="">
      <fullWidth
          link="yoga"
          class="full-width-v-two"
          title="Yoga"
          description="Viens yogater avec le proprio dans divers flow."
          sousdescription="En abonnement ou drop-in."
          textcolor="white"
          imgsrc="img/studio/photo-cours-dan.jpg"
        />
      <div class="container-row">
        <fullWidth
          link="location"
          class="demi-width-v-two"
          title="Location"
          description="Loue l'espace pour ta prochaine activité!"
          textcolor="#FCDA1E"
          imgsrc="img/studio/photo-loue-espace.jpg"
          logosrc=""
        />
        <fullWidth
          link="evenements"
          class="demi-width-v-two"
          title="Événements"
          description="Vient à l'un de nos multiples ateliers, cours de yoga, etc."
          sousdescription=""
          textcolor="black"
          imgsrc="img/studio/photo-cours-dan.jpg"
        />
      </div>
    </div>
  </Layout>
</template>

<script>
import fullWidth from '~/components/fullWidthBloc.vue'

export default {
  components: {
    fullWidth
  },
  metaInfo: {
    title: 'Espace IVY'
  }
}
</script>

<style>

</style>
