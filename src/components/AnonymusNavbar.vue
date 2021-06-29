<template>
  <div>
    <b-navbar id="nav" toggleable="lg" type="dark" class="blue-dark">

      <b-navbar-brand href="#" class="fs-40">
        <b-navbar-toggle class="mr-3" target="nav-collapse"></b-navbar-toggle>
        4Media /
      </b-navbar-brand>
      <b-navbar-nav class="ml-auto d-lg-none">
        <b-nav-item href="#">
          <b-icon icon="search" variant="light"></b-icon>
          <span>Qidirish</span>
        </b-nav-item>
      </b-navbar-nav>

      <b-navbar-nav class="mx-4 d-lg-none">
        <b-nav-item href="#">
          <b-icon icon="bell" variant="light"></b-icon>
        </b-nav-item>

      </b-navbar-nav>
      <b-navbar-nav class="d-lg-none">
        <b-nav-item>
          <b-icon icon="person-square" variant="light"></b-icon>
        </b-nav-item>
      </b-navbar-nav>
      <div class="d-lg-flex d-none">
        <div class="dropdown">
          <a href="#" class="dropbtn">Bosh sahifa</a>
        </div>
        <div class="dropdown">
          <a href="#" class="dropbtn">Kinolar</a>
          <div class="dropdown-content">
            <a href="#">Link 1</a>
            <a href="#">Link 2</a>
            <a href="#">Link 3</a>
          </div>
        </div>
        <div class="dropdown">
          <a href="#" class="dropbtn">Seriallar</a>
          <div class="dropdown-content">
            <a href="#">Link 1</a>
            <a href="#">Link 2</a>
            <a href="#">Link 3</a>
          </div>
        </div>

        <div class="dropdown">
          <a href="#" class="dropbtn">Multfilmlar</a>
          <div class="dropdown-content">
            <a href="#">Link 1</a>
            <a href="#">Link 2</a>
            <a href="#">Link 3</a>
          </div>
        </div>

        <div class="dropdown">
          <a href="#" class="dropbtn">Reytingi yuqori kinolar</a>
          <div class="dropdown-content">
            <a href="#">Link 1</a>
            <a href="#">Link 2</a>
            <a href="#">Link 3</a>
          </div>
        </div>
      </div>


      <b-collapse id="nav-collapse" is-nav>
        <div class="d-flex flex-column d-lg-none">
          <b-navbar-nav>

            <b-nav-item href="#">Bosh sahifa</b-nav-item>

          <b-nav-item-dropdown text="Kinolar">
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item-dropdown text="Seriallar">
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item-dropdown text="Multifilmlar">
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>
          <b-nav-item-dropdown text="Reytingi yuqori kinolar">
            <b-dropdown-item href="#">EN</b-dropdown-item>
            <b-dropdown-item href="#">ES</b-dropdown-item>
            <b-dropdown-item href="#">RU</b-dropdown-item>
            <b-dropdown-item href="#">FA</b-dropdown-item>
          </b-nav-item-dropdown>
          </b-navbar-nav>

        </div>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="ml-auto d-lg-flex d-none">
          <b-nav-item href="#">
            <b-icon icon="search" variant="light"></b-icon>
            <span>Qidirish</span>
          </b-nav-item>


          <b-nav-item href="#">
            <b-icon icon="bell" variant="light"></b-icon>
          </b-nav-item>

          <b-nav-item>
            <b-icon icon="person-square" variant="light"></b-icon>
          </b-nav-item>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>

  </div>
</template>

<script>
export default {
  name: "AnonymusNavbar",
  data() {
    return {}
  },
  methods: {}
}
</script>


<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Prompt&display=swap');

.blue-dark{
  background: #190718;
}


#nav {
  font-family: 'Prompt', sans-serif;
  font-size: 1rem;
}

.fs-40 {
  font-size: 35px;
}


.dropbtn {
  color: white;
  padding: 16px;
  font-size: 16px;
  border: none;
}

.dropdown {
  position: relative;
  display: inline-block;
}


.dropdown-content {
  display: none;
  position: absolute;
  background-color: #f1f1f1;
  min-width: 160px;
  box-shadow: 0px 8px 16px 0px rgba(0, 0, 0, 0.2);
  z-index: 1;
}

.dropdown-content a {
  color: black;
  padding: 12px 16px;
  text-decoration: none;
  display: block;
}

.dropdown-content a:hover {
  background-color: #ddd;
}

.dropdown:hover .dropdown-content {
  display: block;
}

.dropdown:hover .dropbtn {
  color: #FF0040;
}
</style>
