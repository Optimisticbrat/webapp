<template>
  <v-container>
    <v-row class="text-center">
      <v-col cols="12">
        <v-img
          :src="require('../assets/logo_new.png')"
          class="my-3"
          contain
          height="200"
        />
        <v-row justify="center" class="companyname">
          {{ env.title }}
        </v-row>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Main",

  data: () => ({
    env: {
      title: process.env.VUE_APP_TITLE,
      url: process.env.VUE_APP_URL
    }
  })
};
</script>
