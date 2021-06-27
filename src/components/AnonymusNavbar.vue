<template>
  <div>
    <b-navbar id="nav" toggleable="lg" type="dark" variant="dark">
      <b-navbar-brand href="#" class="fs-40">4Media /</b-navbar-brand>
      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav>
          <b-nav-item href="#">Bosh sahifa</b-nav-item>
          <b-nav-item href="#">Kinolar</b-nav-item>
          <b-nav-item href="#">Seriallar</b-nav-item>
          <b-nav-item href="#">Multfilmlar</b-nav-item>
          <b-nav-item href="#">Reytingi eng yuqori</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto">
            <b-nav-item href="#">
              <b-icon icon="search" variant="light"></b-icon>
              <span>Qidirish</span>
            </b-nav-item>


          <b-nav-item href="#"><b-icon icon="bell" variant="light"></b-icon></b-nav-item>

          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content>
              <em><b-icon icon="person-square" variant="light"></b-icon></em>
            </template>
            <b-dropdown-item href="#">Profile</b-dropdown-item>
            <b-dropdown-item href="#">Sign Out</b-dropdown-item>
          </b-nav-item-dropdown>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "AnonymusNavbar"
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Prompt&display=swap');
#nav{
  font-family: 'Prompt', sans-serif;
  font-size: 1rem;
}

.fs-40{
  font-size: 35px;
}
</style>
