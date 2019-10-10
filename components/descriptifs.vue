<template>
  <div :style="'color:' + textcolor +';'" class="descriptifs">
    <h3>{{ title }}</h3>
    <p>{{ description }}</p>
  </div>
</template>

<script>
export default {
  name: 'TextBlock',
  props: {
    title: {
      type: String,
      default: 'IVY'
    },
    imgsrc: {
      type: String,
      default: ''
    },
    description: {
      type: String,
      default: 'Espace IVY'
    },
    textcolor: {
      type: String,
      default: 'black'
    },
    sousdescription: {
      type: String,
      default: ''
    },
    link: {
      type: String,
      default: ''
    }
  },
  data () {
    return {
    }
  }
}
</script>

<style scoped>
.descriptifs {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-evenly;
  text-align: justify;
  max-width: 25vw;
  padding: 0.75rem;
}
@media screen and (max-width: 600px) {
    .descriptifs {
      max-width: 80vw;
    }
}
</style>
