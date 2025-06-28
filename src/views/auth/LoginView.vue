<script setup>
import LoginForm from '@/components/auth/LoginForm.vue'
import AppLayout from '@/components/layout/AppLayout.vue'
</script>

<template>
  <AppLayout>
    <template #content>
      <v-row>
        <v-col cols="12" md="6" class="mx-auto mt-16">
          <v-card class="mx-auto">
            <v-card-title class="text-center">
              <v-img src="/public/images/logo.png" height="200"></v-img>
              <h3 class="font-weight-black">Shirlix Meatshop</h3>
              <p>Login Form</p>
            </v-card-title>

            <v-card-text class="bg-surface-light pt-4">
              <v-divider class="my-5"></v-divider>

              <!-- LOGIN FORM -->
              <LoginForm></LoginForm>

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
