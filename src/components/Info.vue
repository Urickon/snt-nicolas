<template>
  <v-container class="pb-0">
    <v-row class="mb-0">
      <v-col cols="12" md="12" sm="12">
        <v-card
          class="mx-auto"
          flat
        >
          <v-img
            src="../../static/new.png"
            height="500px"
          ></v-img>

          <v-card-text class="display-1 text--primary" id="info">
            Информация о храме
          </v-card-text>
          <v-card-text class="bigCardText">
            <div class="text--primary">
              Храм был построен в 1865 г., являлся центральным во всем районе. В 1935 г. советская власть отобрала храм и переделала его в Дом культуры. с 2006 г., по 2009 г. шло возвращение Храма, местная власть некоторое время препятствовала. Старое здание находилось в аварийном состоянии и было снесено, очищено от мусора. Епископ Магнитогорский и Верхнеуральский Иннокентий благословил на строительство нового здания в данном месте. В ходе расчистки старого здания от мусора в Алтарной части были обнаружены старинные монеты и фрагмент Евангелия. Все артефакты были забетонированы в фундамент.
            </div>
          </v-card-text>
          <v-card-text class="bigCardText">
            <div class="text--primary">
              В процессе восстановления Храму были переданы в дар иконы, утварь от ряда монастырей, храмов, граждан Москвы, г. Бари (Италия), Дивеево, Орска, Задонска, Оптина, Екатеринбурга, Курска, Греции и др. К 2015 году были возведены стены и крыша нового здания. Рядом имеются утерянные захоронения бывших служителей старого храма: протоиерея Николая, протоиерея Евгения и его сына Виталия.            </div>
          </v-card-text>
          <v-divider></v-divider>
          <v-card-text class="mt-8 bigCardText text--primary">
            <strong>Работы, выполненные с 2004 по 2020 год:</strong> вывезли 33 Камаза различного мусора, построили здание 10 м. x 12 м., поставили три купола, построили здание для котельни, сделали внутренную отделку.
          </v-card-text>
          <v-card-text class="mt-2 bigCardText text--primary">
            <p>
              <strong>Мы с Вами сделали в 2021 году:</strong>
            </p>
            <ol>
              <li>Купили котел (дровяной)</li>
              <li>Установили батареи для отопления</li>
              <li>Залили в систему «незамерзайка»</li>
              <li>Поменяли кровлю на Храме</li>
              <li>Сделали котельную и построили дровяник</li>
              <li>Установили Царские Врата</li>
              <li>Пол и потолок обшили ОСВ</li>
              <li>Нам подарили два колокола</li>
            </ol>
          </v-card-text>
          <v-card-text class="mt-2 bigCardText text--primary">
            <p>
              <strong>В 2022 году:</strong>
            </p>
            <ol>
              <li>Сварили новый и мощный котёл</li>
              <li>Переделали подземную тепловую трассу, переделали трубы</li>
              <li>Убрали старый мусор, распилили на дрова прежний сруб</li>
              <li>Покрасили стены</li>
              <li>Привезли икону "Матери  Божией", переданной в дар инок. Макарией</li>
              <li>Залили ж/б., крыльцо</li>
              <li>Обложили плиткой крыльцо и отливы  на отмостках</li>
            </ol>
          </v-card-text>
          <v-card-text class="pt-0 bigCardText text--primary">
            Сейчас нам необходимо 7000 шт. кирпичей и 30 мешков цемента, для того, чтобы построить колокольню.
          </v-card-text>
          <v-card-actions
            class="d-flex justify-center pb-4"
          >
          <a href="#" v-scroll-to="'#charity'">
            <v-btn
              text
              color="green darken-4"
              large
            >
              <strong>Помочь восстановить храм</strong>
            </v-btn>
            </a>
          </v-card-actions>
          <v-divider class="mt-8"></v-divider>
          <v-card-text class="mb-0 pb-0" id="photo">
            <p class="display-1 text--primary">
              Галерея фотографий 
            </p>
          </v-card-text>
          <div>
            <v-row>
              <v-col cols="12" md="12" sm="12">
                <v-card
                  class="mx-auto pa-6"
                  flat
                >
                  <v-row>
                    <v-col
                      v-for="n in 12"
                      :key="n"
                      class="d-flex child-flex"
                      cols="12"
                      md="4"
                      sm="4"
                      xs="12"
                    >
                      <v-img
                        :src="requireImgPath(n)"
                        alt=""
                        aspect-ratio="1"
                        class="grey lighten-2"
                      >
                        <template v-slot:placeholder>
                          <v-row
                            class="fill-height ma-0"
                            align="center"
                            justify="center"
                          >
                            <v-progress-circular
                              indeterminate
                              color="grey lighten-5"
                            ></v-progress-circular>
                          </v-row>
                        </template>
                      </v-img>
                    </v-col>
                  </v-row>
                </v-card>
              </v-col>
            </v-row>
          </div>
          <v-divider class="mt-12"></v-divider>
          <v-card-text class="mb-0 pb-0" id="charity">
            <p class="display-1 text--primary">
              Реквизиты для перечисления платежей
            </p>
          </v-card-text>
          <v-card-text class="ma-0 pb-0">
            <p class="charity__text text--primary specialLineHeight">
              <strong>Рассчетный счет получателя</strong> - 40703810007110002720
            </p>
          </v-card-text>
          <v-divider></v-divider>
          <v-card-title>
            Реквизиты Банка:
          </v-card-title>
          <v-card-text class="mb-0 pb-0 mt-1 pt-1 charity__text text--primary">
            <strong>БИК</strong> - 047501711
          </v-card-text>
          <v-card-text class="mb-0 pb-0 mt-1 pt-1 charity__text text--primary">
            <strong>К/сч</strong> - 30101810400000000711
          </v-card-text>
          <v-card-text class="mt-1 pt-1 charity__text text--primary specialLineHeight">
            <strong>Наименование банка</strong> - ПАО ЧЕЛИНДБАНК г. Челябинск
          </v-card-text>
          <v-divider class="mt-8"></v-divider>
          <v-card-text class="mb-0 pb-0" id="contacts">
            <p class="display-1 text--primary">
              Контакты
            </p>
          </v-card-text>
          <v-card-text class="mb-0">
            <p class="charity__text text--primary">
              <strong>8-951-123-80-13</strong> - настоятель Храма иерей Виталий (Ефремов)
            </p>
            <p class="charity__text text--primary">
              <strong>8-915-022-88-80</strong> - помощник настоятеля Легостаев Виталий Сергеевич
            </p>
          </v-card-text>
          <v-card-text class="mb-6 pt-0">
            <p class="charity__text text--primary specialLineHeight">
              <strong>Адрес храма:</strong> Челябинская область, Карталинский район, п. Елизаветопольское
            </p>
          </v-card-text>
          <v-card-actions
            class="d-flex justify-center pb-10"
          >
            <a href="#" v-scroll-to="'#topElement'">
              <v-btn
                text
                color="green darken-4"
                large
              >
                <strong>Наверх</strong>
              </v-btn>
            </a>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: "Main",
    data () {
      return {
      }
    },
    methods: {
      requireImgPath (n) {
        return require('../../static/'+ n +'.png')
      }
    }
  }
</script>

<style>
  .info-container {
    height: 100%;
    position: relative;
    padding: 2%;
    text-align: justify;
  }
  .info-main-container {
    height: 100%;
    display: flex;
    justify-content: center;
  }
  .charity__text {
    font-size: 24px!important;
  }
  .bigCardText {
    font-size: 20px!important;
  }
  .specialLineHeight {
    line-height: 1.15!important;
  }
  .cardTitleText {
    font-size: 24px!important;
  }
</style>