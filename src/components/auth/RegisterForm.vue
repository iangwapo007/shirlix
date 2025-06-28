<template>
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
        <v-text-field label="Confirm Password" type="password" variant="outlined"></v-text-field
      ></v-col>
    </v-row>

    <v-btn class="mt-2" type="submit" color="red-darken-1" prepend-icon="mdi-account-plus" block
      >Register</v-btn
    >
  </v-form>
</template>
