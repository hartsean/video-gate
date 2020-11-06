<template>
  <div class="container">
    <div>
      <Logo />
      <Video />
      <!-- <div class="featured-video">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/IdWmulnsVQw" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
      </div> -->
      <!-- <Logo2 /> -->
      <div class="links">
        <button
          href="https://stripe.com"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
          v-on:click="buyVideo"
        >
          Watch Video
        </button>
        <button
          href="https://spotify.com"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          Spotify
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      show: false
    }
  },
  methods: {
    buyVideo() {
      console.log('launch paypall')
    }
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
