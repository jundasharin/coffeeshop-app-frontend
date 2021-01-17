<template>
  <div>
    <b-navbar class="navbar" toggleable="lg" type="light" variant="white">
      <b-navbar-brand class="brand" href="#">
        <img
          src="../../assets/icons/coffee-logo.svg"
          class="d-inline-block align-top"
        />
        Coffee Shop
      </b-navbar-brand>

      <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

      <b-collapse id="nav-collapse" is-nav>
        <b-navbar-nav class="mx-auto">
          <b-nav-item href="#">Home</b-nav-item>
          <b-nav-item href="#">Product</b-nav-item>
          <b-nav-item href="#">Your Cart</b-nav-item>
          <b-nav-item href="#">History</b-nav-item>
        </b-navbar-nav>

        <!-- Right aligned nav items -->
        <b-navbar-nav class="navbar-right ml-auto">
          <b-button href="#" variant="white">
            <b-icon icon="search" style="width: 30px; height: 30px;"></b-icon>
          </b-button>
          <b-button class="button-chat" href="#" variant="white">
            <b-badge class="badge-chat" pill variant="primary">1</b-badge>
            <b-icon
              class="icon-chat"
              icon="chat-right-text"
              style="width: 30px; height: 30px;"
            ></b-icon>
          </b-button>

          <b-nav-item-dropdown right>
            <!-- Using 'button-content' slot -->
            <template #button-content class="nav-ava">
              <b-avatar
                style="width: 30px; height: 30px;"
                src="../../assets/icons/user.svg"
              ></b-avatar>
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
  name: "Navbar",
  data() {
    return {
      path: "",
      search: ""
    }
  }
}
</script>
