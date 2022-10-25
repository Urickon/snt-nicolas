<template>
  <v-footer
    padless
  >
    <v-card
      flat
      tile
      class="footer__textBar white--text text-center"
    >
      <v-divider></v-divider>

      <v-card-text class="white--text footer-text-center">
        {{ new Date().getFullYear() }} - <strong> Храм Святого Николая Чудотворца</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
    name: "Footer"
  }
</script>

<style>
.footer-text-center {
  width: 100%;
  display:flex;
  justify-content: center;
  text-align: center;
}
.footer__textBar {
  background-color: #2E7D32!important;
  width: 100%;
  height: 50px;
}
@media screen and (max-width: 600px) {
  .footer-text-center {
    font-size: 12px!important;
  }
}
</style>