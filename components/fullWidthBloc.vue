<template>
  <div class="container-block" :style="'background-image: url(/' + imgsrc + ')'">
    <n-link :style="'color:' + textcolor +';'" class="infos-center-v-two" :to="'/' + link + '/'">
      <h1>{{ title }}</h1>
      <h3>{{ description }} <br> {{ sousdescription }}</h3>
    </n-link>
  </div>
</template>

<script>
export default {
  name: 'FullWidth',
  props: {
    title: {
      type: String,
      default: null
    },
    imgsrc: {
      type: String,
      default: 'img/studio/photo-loue-espace.jpg'
    },
    description: {
      type: String,
      default: null
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
      default: null
    },
    logocolor: {
      type: String,
      default: 'white'
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
.infos-center-v-two {
  position: relative;
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
.reserve {
  display: flex;
  justify-content: center;
  align-items: center;
  border: none;
  color: black;
  background-color: rgba(252, 218, 30, 0.5);
  margin: 0.75rem;
  width: 10rem;
  height: 3rem;
  border-radius: 5px;
  box-shadow: 1px 2px rgba(0, 0, 0, 0.1);
}
.reverse:hover {
  background-color: rgba(252, 218, 30, 1);
}
@media screen and (max-width: 600px) {
    .photo-logo {
      height: -webkit-fill-available;
    }
}
</style>
