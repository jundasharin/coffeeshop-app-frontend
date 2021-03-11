<template>
  <div class="Main">
    <b-row>
      <b-col md="4">
        <Promo />
      </b-col>
      <b-col md="8">
        <Menu />
      </b-col>
    </b-row>
  </div>
</template>

<script>
import Promo from "../_base/Promo"
import Menu from "../_base/Menu"

export default {
  name: "Main",
  components: {
    Promo,
    Menu
  }
}
</script>

<style>
.Main {
  height: 600px;
}
</style>
