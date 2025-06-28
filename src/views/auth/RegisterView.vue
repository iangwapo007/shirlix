<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
import RegisterForm from '@/components/auth/RegisterForm.vue'
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
              <v-divider class="my-5"></v-divider>

              <!-- REGISTER FORM -->
              <RegisterForm></RegisterForm>

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
