<template>
  <div class="home">
    <b-carousel
        id="carousel-1"
        v-model="slide"
        :interval="4000"
        controls
    >
      <b-carousel-slide>
        <template #img>
          <img
              class="d-block bordering px-3 py-3 img-fluid"
              src="https://picsum.photos/1024/480/?image=55"
              alt="image slot"
          >
        </template>
      </b-carousel-slide>
      <b-carousel-slide>
        <template #img>
          <img
              class="d-block bordering px-3 py-3 img-fluid"
              src="https://picsum.photos/1024/480/?image=55"
              alt="image slot"
          >
        </template>
      </b-carousel-slide>
      <b-carousel-slide>
        <template #img>
          <img
              class="d-block bordering px-3 py-3 img-fluid"
              src="https://picsum.photos/1024/480/?image=55"
              alt="image slot"
          >
        </template>
      </b-carousel-slide>

    </b-carousel>
    <div class="follow-pay p-1">
      <p class="text-white pt-2 text-center">14 kun obuna bo'lsih 500 som</p>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  data() {
    return {
      slide: 0,
      sliding: null
    }
  },
  methods: {

  }
}
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Prompt&display=swap');

.bordering {
  border-radius: 1.5rem;
  width: 100%;
  height: 400px;
  object-fit: cover;
}

.follow-pay{
  background: #491a47;
  font-family: 'Prompt', sans-serif;
  margin: 1rem;
}

.follow-pay:hover{
  background: #632760;
  font-family: 'Prompt', sans-serif;
  margin: 1rem;
}


@media (max-width: 900px) {
  .bordering{
    height: 200px;
    object-fit: cover;
  }
}
</style>