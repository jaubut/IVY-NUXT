<template>
  <div :style="'color:' + textcolor +'; background:' + backcolor +';'" class="prices">
      <div class="container-price">
        <h2>{{ title }}</h2>
        <h4>{{ price }}</h4>
        <p>{{ description }}</p>
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
    price: {
      type: String,
      default: '15$'
    },
    description: {
      type: String,
      default: 'Espace IVY'
    },
    textcolor: {
      type: String,
      default: 'black'
    },
    backcolor: {
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
.prices {
  display: flex;
  flex-flow: column wrap;
  justify-content: center;
  text-align: center;
  max-width: 20vw;
  margin: 0.75rem;
  border-radius: 5px;
  border-style: solid;
  border-width: 1px;
  border-color: black;
}
.prices h2 {
    margin: 0;
    padding: 0.75rem 0 0.25rem 0;
}
.prices h4 {
  font-size: 3rem;
  margin: 0;
}
.container-price {
    padding: 0.75rem;
}
@media screen and (max-width: 600px) {
    .prices {
      max-width: 80vw;
    }
}
</style>
