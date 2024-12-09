<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
import LoginForm from '@/components/auth/LoginForm.vue'
</script>

<template>
  <AppLayout>
    <template #content>
      <v-row>
        <v-col cols="12" md="6" class="mx-auto pt-16">
          <v-card class="mx-auto" elavation="24">
            <v-card-text class="text-center">
              <v-img class="mx-auto rounded-circle" src="/images/logo.png" width="25%"></v-img>
              <h1 class="font-weight-black">Skill Hub</h1>
              <p class="font-weight-bold">Login Form</p>
            </v-card-text>

            <v-card-text class="bg-surface-light pt-4">
              <v-divider class="my-5"></v-divider>

              <LoginForm></LoginForm>

              <v-divider class="my-5"></v-divider>

              <h5 class="text-center">
                Don't have to account?
                <RouterLink class="font-weight-black" to="/register">
                  Click here to Register</RouterLink
                >
              </h5>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </template>
  </AppLayout>
</template>
