<template>
  <nav class="nav-sidebar">
    <div class="nav-sidebar__logo-app">
      <img class="nav-sidebar__logo-app__img" src="~/assets/logo.png" alt="" />
    </div>
    <h3>association.name</h3>
    <div class="nav-sidebar__menu-app">
      <NavLink
        linkText="Dashboard"
        route="/"
        fontawesomeIcon="tachometer-alt"
        colorIcon='#673AB7'
      />
      <NavLink linkText="Membres" route="/" fontawesomeIcon="users" colorIcon='#FFC107'/>
      <NavLink linkText="Tournois" route="/" fontawesomeIcon="medal" colorIcon='#009688'/>
      <NavLink
        linkText="Comptabilité"
        route="/"
        fontawesomeIcon="file-invoice-dollar"
        colorIcon='#E91E63'
      />
      <NavLink linkText="Préférences" route="/" fontawesomeIcon="cog" colorIcon='#607D8B'/>
      <hr />
      <h3>Documentation et liens utiles</h3>
      <NavLink linkText="Manuel" route="/" fontawesomeIcon="book" />
      <NavLink linkText="FAQ" route="/" fontawesomeIcon="question" />
      <NavLink linkText="Contact dev" route="/" fontawesomeIcon="headset" />
    </div>
  </nav>
</template>

<script>
export default {}
</script>

<style lang="scss">
.nav-sidebar {
  min-height: 100%;
  display: flex;
  flex-direction: column;
  width: 13%;
  background: $light;
  &__logo-app {
      padding: 1rem;
    &__img {
      width: 100%;
    }
  }
  &__menu-app {
    margin: auto 0;
    display: flex;
    flex-direction: column;
  }
  & hr {
    width: 75%;
  }
  & h3 {
    text-align: center;
  }
}
</style>
