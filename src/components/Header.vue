<template>
  <v-container>
    <v-card class="containerrr">
      <v-card-text class="wrapper py-6" id="topElement">
        <span
          class="font-weight-bold basil--text header--text"
          style="text-align:center;"
        >
          Храм Святителя Николая Чудотворца
        </span>
      </v-card-text>

      <v-tabs
        color="basil"
        grow
        show-arrows
        :vertical="isVertical"
      >
        <v-tab
          class="tab"
        >
          <a href="#" v-scroll-to="'#info'">Информация о храме</a>
        </v-tab>
        <v-tab
          class="tab"
        >
          <a href="#" v-scroll-to="'#photo'">Фотографии</a>
        </v-tab>
        <v-tab
          class="tab"
        >
          <a href="#" v-scroll-to="'#charity'">Пожертвовать</a>
        </v-tab>
        <v-tab
          class="tab"
        >
          <a href="#" v-scroll-to="'#contacts'">Контакты</a>
        </v-tab>
      </v-tabs>
    </v-card>
  </v-container>
</template>

<script>
export default {
  name: 'Header',
  computed: {
    isVertical () {
      return this.$vuetify.breakpoint.name == 'xs' || this.$vuetify.breakpoint.name == 'sm'
    }
  }
}
</script>

<style>
/* Helper classes */
.containerrr {
  background-color: #fafafa;
}
.wrapper {
  display:flex;
  justify-content: center;
  margin-bottom: 16px;
  margin-top: 18px;
  text-align: center;
}
.wrapper > span {
  font-size: 40px!important;
  font-weight: 400;
}
.basil--text {
  color: #356859 !important;
}
.tab {
  background: transparent;
  font-size: 20px!important;
}
.header--text {
  word-wrap: normal!important;
  font-size: 35px!important;
  line-height: 1;
}

@media screen and (max-width: 600px) {
  .tab {
    font-size: 18px!important;
  }
}
</style>
