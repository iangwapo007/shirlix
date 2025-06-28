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
              <v-img src="/public/logo.png" height="270"></v-img>
              <h3 class="font-weight-black">Shirlix Meatshop</h3>
              <p>Register Form</p>
            </v-card-title>

            <v-card-text class="bg-surface-light pt-4">
              <!-- INPUT FORM -->
              <v-divider class="my-5"></v-divider>
              <v-form fast-fail @submit.prevent>
                <v-row>
                  <v-col>
                    <!-- FIRSTNAME FIELD -->
                    <v-text-field label="Firstname" variant="outlined"></v-text-field>
                  </v-col>
                  <v-col>
                    <!-- LASTNAME FIELD -->
                    <v-text-field label="Lastname" variant="outlined"></v-text-field>
                  </v-col>
                </v-row>

                <!-- EMAIL FIELD -->
                <v-text-field label="Email" variant="outlined"></v-text-field>

                <v-row>
                  <v-col>
                    <!-- PASSWORD FIELD -->
                    <v-text-field label="Password" type="password" variant="outlined"></v-text-field
                  ></v-col>
                  <v-col>
                    <!-- CONFIRM PASSWORD FIELD -->
                    <v-text-field
                      label="Confirm Password"
                      type="password"
                      variant="outlined"
                    ></v-text-field
                  ></v-col>
                </v-row>

                <v-btn
                  class="mt-2"
                  type="submit"
                  color="red-darken-1"
                  prepend-icon="mdi-account-plus"
                  block
                  >Register</v-btn
                >
              </v-form>
              <v-divider class="my-5"></v-divider>
              <h5 class="pb-2 text-center">
                Already have an account?
                <RouterLink to="/">Click here to Login</RouterLink>
              </h5>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </template>
  </AppLayout>
</template>
