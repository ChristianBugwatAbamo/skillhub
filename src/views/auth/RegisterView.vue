<script setup>
import AppLayout from '@/components/layout/AppLayout.vue'
import RegisterForm from '@/components/auth/RegisterForm.vue'
</script>

<template>
  <AppLayout>
    <template #content>
      <v-container fluid>
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

                <RegisterForm></RegisterForm>

                <v-divider class="my-5"></v-divider>

                <h5 class="text-center">
                  Already have account? <RouterLink to="/">Click here to Login</RouterLink>
                </h5>
              </v-card-text>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </template>
  </AppLayout>
</template>
