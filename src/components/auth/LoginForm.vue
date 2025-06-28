<template>
  <v-form fast-fail @submit.prevent>
    <v-text-field label="Email" variant="outlined"></v-text-field>

    <v-text-field label="Password" type="password" variant="outlined"></v-text-field>

    <v-btn class="mt-2" type="submit" color="red-darken-1" prepend-icon="mdi-login-variant" block
      >Login</v-btn
    >
  </v-form>
</template>
