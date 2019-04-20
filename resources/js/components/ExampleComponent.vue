<template>
  <div>
    <v-date-picker
      v-model="date"
      width="290"
      class="mt-3"
    ></v-date-picker>
    <v-date-picker
      v-model="date"
      full-width
      landscape
      class="mt-3"
    ></v-date-picker>
  </div>
</template>

<script>
import Vuetify from 'vuetify';
import 'vuetify/dist/vuetify.min.css';
import "vue-material-design-icons/styles.css"
import 'material-design-icons-iconfont/dist/material-design-icons.css'

Vue.use(Vuetify);
  export default {
    data: () => ({
      date: new Date().toISOString().substr(0, 10)
    })
  }
</script>