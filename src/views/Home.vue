<template>
  <div class="Product">
    <Navbar />
    <!-- <img alt="Vue logo" src="../assets/logo.png" />
    <h1>My name is {{ name }}</h1> -->
    <Main />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue"
import Navbar from "../components/_base/Navbar"
import Footer from "../components/_base/Footer"
import Main from "../components/_base/Main"

export default {
  name: "Product",
  components: {
    Navbar,
    Main,
    Footer
  },
  data() {
    return {
      name: "Ahmad Jundan Haris"
    }
  }
}
</script>
