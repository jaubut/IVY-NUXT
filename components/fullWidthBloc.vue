<template>
  <div class="container-block">
    <img :src="imgsrcfinal" class="photo-full" alt="">
    <div class="img-filter" />
    <n-link :style="'color:' + textcolor +';'" class="infos-center" :to="'/' + link + '/'">
      <h1>{{ title }}</h1>
      <h3>{{ description }} <br> {{ sousdescription }}</h3>
    </n-link>
    <img :style="'fill:' + logocolor +';'" class="photo-logo" :src="logosrcfinal" alt="">
  </div>
</template>

<script>
export default {
  name: 'FullWidth',
  props: {
    title: {
      type: String,
      default: 'IVY'
    },
    imgsrc: {
      type: String,
      default: 'img/studio/photo-loue-espace.jpg'
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
    },
    logosrc: {
      type: String,
      default: ''
    },
    logocolor: {
      type: String,
      default: 'white'
    }
  },
  computed: {
    imgsrcfinal () {
      // Return nothing for the default empty string
      if (!this.imgsrc) {
        return
      }

      const fileName = this.imgsrc

      // Request the image as a webpack module by using `require`
      return require(`../assets/${fileName}`)
    },
    logosrcfinal () {
      // Return nothing for the default empty string
      if (!this.logosrc) {
        return
      }

      const fileName = this.logosrc

      // Request the image as a webpack module by using `require`
      return require(`../assets/${fileName}`)
    }
  }
}
</script>

<style scoped>
.container-block {
  transition: all .2s ease-in-out;
}
.photo-full {
  grid-area: 1/1/3/3;
  display: flex;
  justify-content: center;
  align-self: center;
  width: 100%;
  height: auto;
  transition: all .2s ease-in-out;
}
.photo-logo {
  grid-area: 1/1/2/3;
  display: flex;
  align-self: center;
  height: fit-content;
  width: auto;
  z-index: 1;
  margin: auto;
  transition: all .2s ease-in-out;
  color: white;
}
.infos-center {
  grid-area: 1/1/3/3;
  display: flex;
  flex-flow: column wrap;
  justify-content: center;
  align-items: center;
  text-align: center;
  transition: all .2s ease-in-out;
}
.infos-center h3 {
  padding: 0 2.5rem;
}
.img-filter {
  grid-area: 1/1/3/3;
  background: rgba(0,0,0,0.2);
}
@media screen and (max-width: 600px) {
    .full-width {
      margin: 0 2rem 2rem 2rem;
    }
    .photo-logo {
      height: -webkit-fill-available;
    }
}
</style>
