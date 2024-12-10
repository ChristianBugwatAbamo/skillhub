<script setup>
import { ref } from 'vue'

const visible = ref(false)
</script>

<template>
  <v-form fast-fail @submit.prevent>
    <v-text-field label="Email" prepend-inner-icon="mdi-email-outline"></v-text-field>

    <v-text-field
      prepend-inner-icon="mdi-lock-outline"
      label="Password"
      :type="isPasswordVisible ? 'text' : 'password'"
      :append-inner-icon="isPasswordVisible = !isPasswordVisible"
    ></v-text-field>

    <v-btn class="mt-2" type="submit" block color="primary" prepend-icon="mdi-login">Login</v-btn>
  </v-form>
</template>
