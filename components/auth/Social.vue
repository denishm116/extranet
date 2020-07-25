<template>
    <div class="center">
      <v-btn class="ma-2" color="indigo" dark>
        <fa icon="cog" spin/>
      </v-btn>

      <v-btn class="ma-2" color="indigo" prevent dark @click="socialLogin('google')">
        <fa :icon="['fab', 'google']" />
      </v-btn>

      <v-btn class="ma-2" color="indigo" dark @click="socialLogin('yandex')">
        <fa :icon="['fab', 'yandex']" />
      </v-btn>

      <v-btn class="ma-2" color="indigo" dark @click="socialLogin('facebook')">
        <fa :icon="['fab', 'facebook-f']" />
      </v-btn>

      <v-btn class="ma-2" color="indigo" dark @click="socialLogin('vkontakte')">
        <fa :icon="['fab', 'vk']" />
      </v-btn>

   </div>
</template>

<script>

    export default {
methods: {
  socialLogin(service) {
    window.location.href = `${process.env.baseUrl}auth/login/${service}`;
  }
}



    }
</script>

<style scoped>
.center {
  margin: 0 auto;
}
</style>
