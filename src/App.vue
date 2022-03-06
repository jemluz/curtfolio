<template>
  <div id="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view/>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Changa:wght@400;500&family=Coustard&display=swap');
@import './styles/styles.scss';

#app {
  font-family: $coustardFont;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  color: $gray;
}

* {
  margin: 0px;
  padding: 0px;
  font-weight: 400;
}

</style>
