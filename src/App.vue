<template>
  <div id="app">
    <div id="nav">
      <AnonymusNavbar msg="Welcome to Your Vue.js App"/>
    </div>
    <router-view/>
  </div>
</template>

<style>

</style>
<script>
import AnonymusNavbar from "@/components/AnonymusNavbar";
export default {
  components: {AnonymusNavbar}
}
</script>