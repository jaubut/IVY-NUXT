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
    </div>
  </Layout>
</template>

<script>
import fullWidth from '~/components/fullWidthBloc.vue'

export default {
  components: {
    fullWidth
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
</style>
