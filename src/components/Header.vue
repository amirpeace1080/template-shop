<template>
  <div class="navbar-main">
    <!-- size lg -->
    <v-app-bar class="hidden-sm-and-down" color="white" fixed>
      <v-toolbar-items>
        <v-btn text to="/">
          <v-icon>mdi-account</v-icon>
        </v-btn>
        <v-btn text to="/aa">
          <v-icon>mdi-cart</v-icon>
        </v-btn>
        <v-btn text to="/about">
          <v-icon>mdi-home</v-icon>
        </v-btn>
        <v-btn>
          <v-icon>mdi-search-web</v-icon>
        </v-btn>
      </v-toolbar-items>
      <v-spacer></v-spacer>

      <v-toolbar-items>
        <v-btn class="sign">
          <v-icon>mdi-account</v-icon>
        <router-link to="/login">ثبت نام / ورود</router-link>
        </v-btn>
      </v-toolbar-items>
    </v-app-bar>

    <!-- size mobile -->
    <v-app-bar class="hidden-sm-and-up" color="white" fixed>
      <v-app-bar-nav-icon @click="drawer = true"></v-app-bar-nav-icon>
      <v-spacer></v-spacer>
      <v-btn class="sign">
        <v-icon>mdi-account</v-icon>
        <router-link to="/login">ثبت نام / ورود</router-link>
      </v-btn>
    </v-app-bar>

    <v-navigation-drawer v-model="drawer" absolute temporary>
      <v-system-bar></v-system-bar>
      <v-list>
        <v-list-item>
          <v-list-item-avatar>
            <v-img
              src="https://lh3.googleusercontent.com/a-/AOh14GhRowOcRCeXt5Uw7plDEq6qacBrFbyjB-UQ7txUbw=s96-c-rg-br100"
            ></v-img>
          </v-list-item-avatar>
        </v-list-item>

        <v-list-item link>
          <v-list-item-content>
            <v-list-item-title class="text-h6">
              Mohammad Sharifi
            </v-list-item-title>
            <v-list-item-subtitle>amirpeace1080@gmail.com</v-list-item-subtitle>
          </v-list-item-content>

          <v-list-item-action>
            <v-icon>mdi-menu-down</v-icon>
          </v-list-item-action>
        </v-list-item>
      </v-list>
      <v-divider></v-divider>
      <v-list nav dense>
        <v-list-item-group color="primary">
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title>
                <v-icon>mdi-account</v-icon>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title>
                <v-icon>mdi-cart</v-icon>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title>
                <v-icon>mdi-home</v-icon>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-content>
              <v-list-item-title>
                <v-icon>mdi-search-web</v-icon>
              </v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list-item-group>
      </v-list>

      <!-- <template v-slot:append>
        <div class="pa-2">
          <v-btn block @click="logout"> Logout </v-btn>
        </div>
      </template> -->
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,
      group: null,
    };
  },
};
</script>

<style scoped>
.sign {
  border: 1px solid #000;
  background-color: #fff;
}
</style>