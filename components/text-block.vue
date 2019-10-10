<template>
  <div>
    <div :style="'color:' + textcolor +';'" class="infos-center">
      <h1>{{ title }}</h1>
      <h3>{{ description }} <br> {{ sousdescription }}</h3>
    </div>
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
.infos-center {
  grid-area: 1/1/3/3;
  display: flex;
  flex-flow: column wrap;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.infos-center h3 {
  padding: 0 2.5rem;
}
@media screen and (max-width: 600px) {
}
</style>
