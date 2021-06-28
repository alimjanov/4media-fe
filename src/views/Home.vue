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
.bordering {
  border-radius: 1.5rem;
  width: 100%;
  height: 400px;
}
</style>