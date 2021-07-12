<template>
  <v-app>
    <v-app-bar
      color="#00C853"
      dark
    >
    <v-app-bar-nav-icon @click.stop="drawer = !drawer" class="hidden-md-and-up"></v-app-bar-nav-icon>
    <v-toolbar-title
        black--text
        font-weight-bold
      >Zalisha</v-toolbar-title>

      <v-spacer></v-spacer>

      <v-btn
        target="_blank"
        text
        class="hidden-sm-and-down"
      >
        <v-icon>mdi-account</v-icon>
        <span class="mr-2">FARMERS</span>
      </v-btn>

      <v-btn
        target="_blank"
        text
        class="hidden-sm-and-down"
      >
        <v-icon>mdi-storefront</v-icon>
        <span class="mr-2">BUSINESSES</span>
      </v-btn>

      <v-btn
        target="_blank"
        text
        class="hidden-sm-and-down"
      >
        <v-icon>mdi-cart</v-icon>
        <span class="mr-2">MARKETPLACE</span>
      </v-btn>
    </v-app-bar>

    <v-navigation-drawer app v-model="drawer">
      <v-list-item-group
       v-model="group"
      >
          <v-list-item>
            <v-list-item-title><v-icon>mdi-home</v-icon>Home</v-list-item-title>
          </v-list-item>
           <br>
          <v-list-item>
            <v-list-item-title><v-icon>mdi-storefront</v-icon>BUSINESSES</v-list-item-title>
          </v-list-item>
           <br>
          <v-list-item>
            <v-list-item-title><v-icon>mdi-cart</v-icon>MARKETPLACE</v-list-item-title>
          </v-list-item>
         </v-list-item-group> 
    </v-navigation-drawer>
   
    <v-main>
      <router-view/>
       <v-footer style="background-color: #00695C; max-width:auto; margin-left: 0;">
  
    <v-row class="hidden-sm-and-down">
      <v-col>
      <v-card color="#00695C" dark outlined>
         <v-card-title>
           ZALISHA
         </v-card-title>
         <v-card-text>Farmers Platform</v-card-text>
         <v-card-text>Zalisha for Businesses</v-card-text>
         <v-card-text>Marketplace</v-card-text>
         <v-card-text>Privacy</v-card-text>
      </v-card>
      </v-col>

     <v-col>
      <v-card color="#00695C" dark outlined>
         <v-card-title>
           COMPANY
         </v-card-title>
         <v-card-text>About</v-card-text>
         <v-card-text>Get in touch</v-card-text>
         <v-card-text>Media</v-card-text>
         <v-card-text>Privacy & Terms</v-card-text>
      </v-card>
      </v-col>

     <v-col>
      <v-card color="#00695C" dark outlined>
         <v-card-title>
           CONTACTS
         </v-card-title>
         <v-card-subtitle><v-icon>mdi-email</v-icon><strong>Mail</strong></v-card-subtitle>
         <v-card-text>info@zalishafrica.com</v-card-text>
         <v-card-text>engineering@fineteklabs.com</v-card-text>
         <v-divider></v-divider>
         <v-card-subtitle><v-icon>mdi-phone</v-icon><strong>Telephone</strong></v-card-subtitle>
         <v-card-text>Telephone 1: <a href="tel: 0734-341-962">+254 734 34 1962</a></v-card-text>
         <v-card-text>Telephone 2: <a href="tel:  0706-05-99-06">+254 706 059 906</a></v-card-text>
      </v-card>
      </v-col>

     <v-col>
      <v-card color="#00695C" dark outlined>
        <v-card-title>SOCIALS</v-card-title>
        <v-card-actions>
          <v-row>
            <v-col>
            <v-btn
              icon
            >
              <a href="https://facebook.com/zalishafrica" style="color: white;"><v-icon>mdi-facebook</v-icon></a>
            </v-btn>
          </v-col>

          <v-col>
            <v-btn
              icon
            >
              <a href="https://twitter.com/zalishafrica" style="color: white;"><v-icon>mdi-twitter</v-icon></a>
            </v-btn>
          </v-col>

          <v-col>
            <v-btn
              icon>
              <a href="https://instagram.com/zalishafrica" style="color: white;"><v-icon>mdi-instagram</v-icon></a>
            </v-btn>
          </v-col>

          <v-col
            cols="12"
            sm="3"
          >
            <v-btn
              icon
            >
              <a href="https://linkedin.com/company/zalisha" style="color: white;"><v-icon>mdi-linkedin</v-icon></a>
            </v-btn>
          </v-col>
          </v-row>
        </v-card-actions>
      </v-card>
      </v-col>
</v-row>

<v-col class="hidden-md-and-up">
      <v-row class="d-flex justify-center mb-6">
      <v-card color="#00695C" dark outlined>
         <v-card-title>
           ZALISHA
         </v-card-title>
         <v-card-text>Farmers Platform</v-card-text>
         <v-card-text>Zalisha for Businesses</v-card-text>
         <v-card-text>Marketplace</v-card-text>
         <v-card-text>Privacy</v-card-text>
      </v-card>
      </v-row>

     <v-row style="padding-right: 28px;">
      <v-card color="#00695C" dark outlined>
         <v-card-title>
           COMPANY
         </v-card-title>
         <v-card-text>About</v-card-text>
         <v-card-text>Get in touch</v-card-text>
         <v-card-text>Media</v-card-text>
         <v-card-text>Privacy & Terms</v-card-text>
      </v-card>
      </v-row>

     <v-row>
      <v-card color="#00695C" dark outlined>
         <v-card-title>
           CONTACTS
         </v-card-title>
         <v-card-subtitle><v-icon>mdi-email</v-icon><strong>Mail</strong></v-card-subtitle>
         <v-card-text>info@zalishafrica.com</v-card-text>
         <v-card-text>engineering@fineteklabs.com</v-card-text>
         <v-divider></v-divider>
         <v-card-subtitle><v-icon>mdi-phone</v-icon><strong>Telephone</strong></v-card-subtitle>
         <v-card-text>Telephone 1: <a href="tel: 0734-341-962">+254 734 34 1962</a></v-card-text>
         <v-card-text>Telephone 2: <a href="tel:  0706-05-99-06">+254 706 059 906</a></v-card-text>
      </v-card>
      </v-row>

     <v-row>
      <v-card color="#00695C" dark outlined>
        <v-card-title>SOCIALS</v-card-title>
        <v-card-actions>
          <v-row>
            <v-col>
            <v-btn
              icon
              class="white--text"
            >
              <a href="https://facebook.com/zalishafrica" style="color: white;"><v-icon>mdi-facebook</v-icon></a>
            </v-btn>
          </v-col>

          <v-col>
            <v-btn
              icon
            >
              <a href="https://twitter.com/zalishafrica" style="color: white;"><v-icon>mdi-twitter</v-icon></a>
            </v-btn>
          </v-col>

          <v-col>
            <v-btn
              icon>
              <a href="https://instagram.com/zalishafrica" style="color: white;"><v-icon>mdi-instagram</v-icon></a>
            </v-btn>
          </v-col>

          <v-col
            cols="12"
            sm="3"
          >
            <v-btn
              icon
            >
              <a href="https://linkedin.com/company/zalisha" style="color: white;"><v-icon>mdi-linkedin</v-icon></a>
            </v-btn>
          </v-col>
          </v-row>
        </v-card-actions>
      </v-card>
      </v-row>
</v-col>
    </v-footer>


    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  data: () => ({
    drawer: false,
    group: null,
  }),
  watch: {
      group () {
        this.drawer = false
      },
    },
};
</script>
<style>
a{
  text-decoration: none;
}
</style>