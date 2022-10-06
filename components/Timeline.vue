<template>
  <div>
    <v-toolbar
      elevation="4"
    >
      <v-toolbar-title> Página Inicial </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn icon>
      <v-icon>mdi-star-four-points-outline</v-icon>
      </v-btn>
    </v-toolbar>
    <v-list three-line>

      <template v-for="(tweet, index) in tweets">
        <v-subheader
          v-if="tweet.header"
          :key="tweet.header"
          v-text="tweet.header"
        ></v-subheader>

        <v-divider
          v-else-if="tweet.divider"
          :key="index"
          :inset="tweet.inset"
        ></v-divider>

        <v-list-item
          v-else
          :key="tweet.title"
        >
          <v-list-item-avatar>
            <v-img :src="tweet.avatar"></v-img>
          </v-list-item-avatar>

          <v-list-item-content>
            <v-list-item-title>
              <nuxt-link :to="{ name: 'user-username', params: { username: tweet.username }}">{{tweet.name}}  {{tweet.username}}</nuxt-link>
              {{tweet.data}} <v-btn icon>
                <v-icon>mdi-settings-helper</v-icon>
              </v-btn> </v-list-item-title>
              <v-list-item-subtitle v-html="tweet.text"></v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </template>
    </v-list>
  </div>
</template>

<script>
export default {
  name: 'TimeLine',
  props: ['tweets'],
  data () {
    return {}
  }
}
</script>
