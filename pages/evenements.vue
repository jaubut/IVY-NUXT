<template>
  <Layout>
    <div>
      <fullWidth
        class="full-width-v-two"
        title="Évènements"
        description="Soit au courant de tous les événements IVY"
        textcolor="black"
        link="location"
        imgsrc="img/studio/photo-loue-espace.jpg"
      />
      <div class="container-facebook">
        <div
          class="fb-page"
          data-href="https://www.facebook.com/espaceivy/"
          data-tabs="events"
          data-width="500"
          data-height=""
          data-small-header="true"
          data-adapt-container-width="true"
          data-hide-cover="false"
          data-show-facepile="true"
        >
          <blockquote cite="https://www.facebook.com/espaceivy/" class="fb-xfbml-parse-ignore">
            <a href="https://www.facebook.com/espaceivy/">Ivy Espace Yoga - Arts &amp; Communauté</a>
          </blockquote>
        </div>
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
  mounted () {
    this.$initFbSDK()
  }
}
</script>

<style scoped>
.container-facebook {
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
