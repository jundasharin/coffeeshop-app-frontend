<template>
  <div class="Product">
    <Navbar />
    <img alt="Vue logo" src="../assets/logo.png" />
    <h1>My name is {{ name }}</h1>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue"
import Navbar from "../components/_base/Navbar"

export default {
  name: "Product",
  components: {
    Navbar
  },
  data() {
    return {
      name: "Ahmad Jundan Haris"
    }
  }
}
</script>
