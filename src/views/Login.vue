<template>
  <!-- <v-card elevation="4"></v-card> -->
  <v-container class="fill-height">
    <v-layout class="align-center justify-center">
      <v-flex class="login-form text-xs-center">
        <div class="display-1 mb-3">
          صفحه ورود
        </div>
        <v-card elevation="12">
          <v-card-text>
            <div class="subheading">
              <template v-if="options.isLoggingIn"
                >صفحه ورود مشتریان</template
              >
              <template v-else>ساخت اکانت جدید</template>
            </div>
            <v-form>
              <v-text-field
                v-if="!options.isLoggingIn"
                v-model="user.name"
                light="light"
                prepend-icon="mdi-account"
                label="نام"
              ></v-text-field>
              <v-text-field
                v-model="user.email"
                light="light"
                prepend-icon="mdi-email"
                label="ایمیل"
                type="email"
              ></v-text-field>
              <v-text-field
                v-model="user.password"
                light="light"
                prepend-icon="mdi-lock"
                label="رمز عبور"
                type="password"
              ></v-text-field>
              <v-checkbox
                v-if="options.isLoggingIn"
                v-model="options.shouldStayLoggedIn"
                light="light"
                label="مرا بخاطر بسپار"
                hide-details="hide-details"
              ></v-checkbox>
              <v-btn
                v-if="options.isLoggingIn"
                @click.prevent=""
                block="block"
                type="submit"
                >ورود</v-btn
              >
              <v-btn v-else
                block="block" type="submit" @click.prevent="options.isLoggingIn
                = true">ایجاد حساب</v-btn
              >
            </v-form>
          </v-card-text>
        </v-card>
        <div class="mt-4" v-if="options.isLoggingIn">
          حساب کاربری ندارید؟
          <v-btn light="light" @click="options.isLoggingIn = false"
            >ایجاد حساب</v-btn
          >
        </div>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
export default {
  data() {
    return {
      user: {
        name: null,
        email: null,
        password: null,
      },
      options: {
        isLoggingIn: true,
        shouldStayLoggedIn: true,
      },
    };
  },
};
</script>

<style scoped>
.login-form {
  max-width: 500px;
}
</style>