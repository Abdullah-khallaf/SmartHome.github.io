<template>
  <div class="header">
    <div id="nav">
      <b-navbar toggleable="lg"  class="navbar">
          <div class="container">
        <b-navbar-brand href="#">FEE Smart Home</b-navbar-brand>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

        <b-collapse id="nav-collapse" is-nav>
          <b-navbar-nav>
            <b-nav-item href="#">Home <i class="fas fa-home"></i> |</b-nav-item>

            <b-nav-item href="#"
              >Notification <i class="far fa-bell"></i> |
            </b-nav-item>
            <b-nav-item href="#"
              >Temperature <i class="fas fa-thermometer-three-quarters"></i> |
            </b-nav-item>
            <b-nav-item href="#"
              >Controllers <i class="fas fa-sliders-h"></i>
            </b-nav-item>
          </b-navbar-nav>

          <!-- Right aligned nav items -->
          <b-navbar-nav class="ml-auto"> </b-navbar-nav>
        </b-collapse>
        </div>
      </b-navbar>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppHeader",
};
</script>
<style lang="scss" scoped>
.navbar {
  background-color: #3370a6;
  
  .navbar-brand {
      margin-right: 20%;
    font-family: sans-serif ;
    font-weight: bold;
    font-size: 27px;
    color: #1c3659 ;
    text-shadow: 0px 1px 1px    rgba(0, 0, 0, 0.705) (0, 0, 0, 0.705)
      (0, 0, 0, 0.973) ;
      &:hover{
         color: #0b1f3a; 
      }
  }
  .navbar-nav {
      
    .nav-item {
      font-family: sans-serif ;
      font-weight: bold;
      font-size: 20px;
      color: #1c3659 ;
      text-shadow: 0px 1px 1px rgba(0, 0, 0, 0.705) (0, 0, 0, 0.705)
        (0, 0, 0, 0.973);
        &:hover{
         color: #0b1f3a; 
      }
    }
  }
}
</style>
