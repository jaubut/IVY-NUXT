<template>
  <div class="container-photos">
    <div class="photos photo-un" :style="'background-image: url(/' + imgsrcun + '?nf_resize=fit)'" />
    <div class="photos photo-deux" :style="'background-image: url(/' + imgsrcdeux + '?nf_resize=fit)'" />
    <div class="photos photo-trois" :style="'background-image: url(/' + imgsrctrois + '?nf_resize=fit)'" />
    <div class="photos photo-quatre" :style="'background-image: url(/' + imgsrcquatre + '?nf_resize=fit)'" />
    <div class="photos photo-cinq" :style="'background-image: url(/' + imgsrccinq + '?nf_resize=fit)'" />
  </div>
</template>

<script>
export default {
  props: {
    imgsrcun: {
      type: String,
      default: null
    },
    imgsrcdeux: {
      type: String,
      default: null
    },
    imgsrctrois: {
      type: String,
      default: null
    },
    imgsrcquatre: {
      type: String,
      default: null
    },
    imgsrccinq: {
      type: String,
      default: null
    }
  }
}
</script>

<style scoped>
.container-photos {
    display: grid;
    grid-template: 1fr 1fr 1fr / 1fr 1fr 1fr;
    grid-gap: 0.75rem;
    margin: 0 2rem 2rem 2rem;
    min-height: 35vh;
}
.photos {
    background-repeat: no-repeat;
    background-position: center;
    background-size: cover;
}
.photo-un {
    grid-area: 1/1/3/2;
}
.photo-deux {
    grid-area: 1/2/2/4;
}
.photo-trois {
    grid-area: 2/2/3/3;
}
.photo-quatre {
    grid-area: 3/1/4/3;
}
.photo-cinq {
    grid-area: 2/3/4/4;
}
</style>
