<template>
  <router-view />
</template>
<style lang="scss">
@import "./assets/scss/_variables.scss";
@font-face {
  font-family: Mulish;
  src: url("./assets/fonts/Mulish-VariableFont_wght.ttf") format("truetype");
  font-weight: 200 900;
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Mulish, sans-serif;
  color: $dark-shades;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
