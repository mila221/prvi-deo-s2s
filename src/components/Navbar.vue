<template>
    <div>
        <v-toolbar color="primary" dark>
            <v-app-bar-nav-icon @click="drawer = !drawer" class="hidden-sm-and-up"></v-app-bar-nav-icon>
            <v-spacer></v-spacer>
            <v-toolbar-items class="hidden-xs-only">
                <v-btn text to="/">Home</v-btn>
                <v-btn text to="/posts">Posts</v-btn>
                <v-btn text>User</v-btn>
                <v-btn text>Contact</v-btn>
            </v-toolbar-items>
        </v-toolbar>
        <v-navigation-drawer v-model="drawer" absolute>
            <v-list>
                <v-list-item active-class="primary--text" to="/">Home</v-list-item>
                <v-list-item active-class="primary--text" to="/posts">Posts</v-list-item>
                <v-list-item active-class="primary--text" to="/user">User</v-list-item>
                <v-list-item active-class="primary--text" to="/contact">Contact</v-list-item>
            </v-list>
        </v-navigation-drawer>
  </div> 
</template>
<script>
export default {
  data(){
    return {
      drawer: false
    }
  }
}
</script>