<template>
  <div id="app">
    <b-navbar toggleable="md" variant="dark" type="dark">
      <b-navbar-toggle target="nav_collapse"></b-navbar-toggle>
      <img src="./assets/logo.png" class="img-circle" style="padding: 5px">
      <b-navbar-brand>MyMovie</b-navbar-brand>
      <b-collapse is-nav id="nav_collapse">
        <b-navbar-nav>
          <b-nav-item to="/"><i class="fa fa-home" style="padding: 5px"> Home</i></b-nav-item>
          <b-nav-item to="/slide"><i class="fa fa-list" style="padding: 5px"> Movie </i></b-nav-item>
          <b-nav-item to="/movie"><i class="fa fa-list" style="padding: 5px"> VoteRank</i></b-nav-item>
          <b-nav-item to="/addMovie"><i class="fa fa-list" style="padding: 5px"> Add Movie </i></b-nav-item>
        </b-navbar-nav>
        <b-navbar-nav class="ml-auto">
          <b-nav-item to="/login"><i class="fa fa-comment" style="padding: 5px"> Login </i></b-nav-item>
          <b-nav-item to="/logout"><i class="fa fa-sign-out" style="padding: 5px"> Logout </i></b-nav-item>
          <i class="fa fa-pied-piper-alt fa-1x" style="padding: 5px; color: white;"></i>
        </b-navbar-nav>
      </b-collapse>
    </b-navbar>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
  #app {
    font-family: 'Avenir', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: aliceblue;
    padding-top: 20px;
    background: url("./assets/timg.jpeg")no-repeat;
    background-size: auto 100%;
  }
  .VueTables__sortable {
    cursor: pointer;
  }
</style>
