<template>
  <Home :tweets='tweets' />
</template>

<script>
import Home from '../components/Home.vue'

export default {
  name: 'IndexPage',
  data () {
    return {
      tweets: [
        {
          avatar: 'https://cdn.vuetifyjs.com/images/lists/1.jpg',
          name: 'Brunch this weekend?',
          username: '@qualquer',
          data: '4 de outubro',
          text: 'blablabla',
          subtitle: 'sdcfsdvfsddgfsd'
        },
        { divider: true, inset: true },
        {
          avatar: 'https://cdn.vuetifyjs.com/images/lists/2.jpg',
          name: 'Brunch this weekend?',
          username: '@qualquer',
          data: '4 de outubro',
          text: 'blablabla',
          subtitle: 'sdcfsdvfsddgfsd'

        },
        { divider: true, inset: true },
        {
          avatar: 'https://cdn.vuetifyjs.com/images/lists/3.jpg',
          name: 'Brunch this weekend?',
          username: '@qualquer',
          data: '4 de outubro',
          text: 'blablabla',
          subtitle: 'sdcfsdvfsddgfsd'
        }
      ]
    }
  },
  components: {
    Home
  }
}
</script>
