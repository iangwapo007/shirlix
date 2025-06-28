<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
</script>

<template>
  <AppLayout>
    <template #content>
      <v-row>
        <v-col cols="12" md="6" class="mx-auto mt-16">
          <v-card class="mx-auto">
            <v-card-title class="text-center">
              <v-img src="/public/logo.png" height="200"></v-img>
              <h3 class="font-weight-black">Shirlix Meatshop</h3>
              <p>Login Form</p>
            </v-card-title>

            <v-card-text class="bg-surface-light pt-4">
              <v-divider class="my-5"></v-divider>
              <v-form fast-fail @submit.prevent>
                <v-text-field label="Email" variant="outlined"></v-text-field>

                <v-text-field label="Password" type="password" variant="outlined"></v-text-field>

                <v-btn
                  class="mt-2"
                  type="submit"
                  color="red-darken-1"
                  prepend-icon="mdi-login-variant"
                  block
                  >Login</v-btn
                >
              </v-form>

              <v-divider class="my-5"></v-divider>

              <h5 class="pb-2 text-center">
                Dont have an Account?
                <RouterLink to="/register">Click here to register</RouterLink>
              </h5>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </template>
  </AppLayout>
</template>
