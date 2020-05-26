<template>
  <v-app>

    <v-navigation-drawer style="background-color: #005e8a !important;" dark app>
      
      <v-list dense nav>
        <v-list-item-group color="beige">
        <v-list-item v-for="item in items" :key="item.title" :to="item.link"  >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item-content>
        </v-list-item>
        </v-list-item-group>
      </v-list>

    </v-navigation-drawer>


  <div class="layout">
    <header class="header">
      <v-img alt="Example image" src="https://gridsome.org/logos/logo-normal.svg" width="300" style="margin-right: 10px; margin-top: 20px;" />
    </header>
    <article>
    <slot/>
    </article>
  </div>
  </v-app>
</template>

<static-query>
query {
  metadata {
    siteName
  }
}
</static-query>

<style>

body {
  font-family: -apple-system,system-ui,BlinkMacSystemFont,"Segoe UI",Roboto,"Helvetica Neue",Arial,sans-serif;
  margin:0;
  padding:0;
  line-height: 1.5;
}

.layout {
  display: block;
  max-width: 760px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
}

.header {
  display: block;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  height: 80px;
}

.nav {
  display: inline;
}

.nav__link {
  margin-left: 20px;
}
</style>

<script>
export default {
  data() {
    return {
      items: [
        { title: 'Home', icon: 'mdi-apps', link: '/' },
        { title: 'About', icon: 'mdi-apps', link: '/about' },
        { title: 'Contact', icon: 'mdi-apps', link: '/contact' }
      ],
      clipped: false,
      drawer: true,
      right: null,
      group: null,
    }
  }
}
</script>