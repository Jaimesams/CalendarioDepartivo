<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/neon.png" class="img" />
  </div>
  <div class="container">
    <CuerpoIndex />
    <BotonesPrincipales />
    <MenuBoton @Alt-Menu="AltMenu" />
  </div>
</template>

<script>
import CuerpoIndex from "@/components/CuerpoIndex.vue";
import BotonesPrincipales from "@/components/BotonesPrincipales.vue";
import MenuBoton from "@/components/MenuBoton.vue";

export default {
  name: "App",
  components: {
    CuerpoIndex,
    BotonesPrincipales,
    MenuBoton,
  },
};
</script>

<style Lang="scss">
:root {
  --background-body: #423a3a;
}
#app {
  display: flex;
  height: 100vh;
  padding: 5px;
  font-family: "Helvetica", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  margin: 0;
  .img {
    width: 1052px;
    height: auto;
    margin: 10px;
    background-size: contain;
    position: fixed;
    top: 50%;
    left: 48%;
    transform: translate(-50%, -43%);
    width: 100%;
    height: 115%;
    z-index: -1;
  }
}
body {
  margin: 0;
  background-color: #0c0000;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 2000 1500'%3E%3Cdefs%3E%3Cpath fill='none' stroke-width='3.9' stroke-opacity='.51' id='a' d='M0.85-507.63l485.39 352.65l-185.4 750.61h-50.1000-350.4-570.61L0.74-509.63 M0.74-950.87l-486.56 353.51l185.85 501.99h601.42L487.3-257.36L80.74-510.87L0.74-510.87z'/%3E%3C/defs%3E%3Cg transform='scale(0.905)' style='transform-origin:center'%3E%3Cg transform='rotate(8.48 0 0)' style='transform-origin:right'%3E%3Cg transform='rotate(-108.8 0 0)' style='transform-origin:center'%3E%3Cg transform='translate(1000 750)'%3E%3Cuse stroke='%2B010B' href='%23a' transform='rotate(1.8 0 0) scale(1.068)'/%3E%3Cuse stroke='%2348010c' href='%23a' transform='rotate(13.6 0 0) scale(1.136)'/%3E%3Cuse stroke='%2355010d' href='%23a' transform='rotate(20.4 0 0) scale(1.204)'/%3E%3Cuse stroke='%2362010f' href='%23a' transform='rotate(27.2 0 0) scale(1.272)'/%3E%3Cuse stroke='%236f0110' href='%23a' transform='rotate(34 0 0) scale(1.34)'/%3E%3Cuse stroke='%237c0111' href='%23a' transform='rotate(40.8 0 0) scale(1.408)'/%3E%3Cuse stroke='%23890112' href='%23a' transform='rotate(47.6 0 0) scale(1.476)'/%3E%3Cuse stroke='%23960113' href='%23a' transform='rotate(54.4 0 0) scale(1.544)'/%3E%3Cuse stroke='%23a40015' href='%23a' transform='rotate(61.2 0 0) scale(1.612)'/%3E%3Cuse stroke='%23b10016' href='%23a' transform='rotate(68 0 0) scale(1.68)'/%3E%3Cuse stroke='%23be0017' href='%23a' transform='rotate(74.8 0 0) scale(1.748)'/%3E%3Cuse stroke='%23cb0018' href='%23a' transform='rotate(81.6 0 0) scale(1.816)'/%3E%3Cuse stroke='%23d80019' href='%23a' transform='rotate(88.4 0 0) scale(1.884)'/%3E%3Cuse stroke='%23e5001b' href='%23a' transform='rotate(95.2 0 0) scale(1.952)'/%3E%3Cuse stroke='%23f2001c' href='%23a' transform='rotate(102 0 0) scale(2.02)'/%3E%3Cuse stroke='%23FF001D' href='%23a' transform='rotate(108.8 0 0) scale(2.088)'/%3E%3C/g%3E%3C/g%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
  background-attachment: fixed;
  background-size: cover;
}

body::after {
  content: "";
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 65%;
  height: 65%;
  background: url("./assets/UFCIndex.png") center center no-repeat fixed;
  background-size: contain;
  z-index: -1;
}
</style>
