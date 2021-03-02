<template>
  <router-view />
</template>
<style lang="scss">
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
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

// Variables
$light-shades: #f0f1f1;
$light-accent: #779c9c;
$main: #10b981;
$dark-accent: #6c6e6e;
$dark-shades: #1e2027;
$primary: #0ebf7f;
$info: #1e2027;
$success: #39b45e;
$warning: #b7a426;
$danger: #f44336;
</style>
