<template>
<div>
   <v-card
      elevation="12"
      width="256"
    >
      <v-navigation-drawer
        floating
        permanent
      >
        <v-list
          dense
          rounded
        >
          <v-list-item
            v-for="item in items"
            :key="item.title"
            link
          >
            <v-list-item-icon>
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-item-icon>

            <v-list-item-content>
              <v-list-item-title>{{ item.title }}</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
        </v-list>
      </v-navigation-drawer>
      <v-btn>
            Tweet
      </v-btn>
    </v-card>
</div>
</template>

<script>

export default {
  name: 'MenuPage',
  data () {
    return {
      items: [
        { title: 'Home', icon: 'mdi-view-dashboard' },
        { title: 'Explore', icon: 'mdi-forum' },
        { title: 'Notifications', icon: 'mdi-forum' },
        { title: 'Messages', icon: 'mdi-forum' },
        { title: 'Bookmarks', icon: 'mdi-forum' },
        { title: 'List', icon: 'mdi-forum' },
        { title: 'Profile', icon: 'mdi-forum' },
        { title: 'More', icon: 'mdi-forum' }
      ]
    }
  }
}
</script>
