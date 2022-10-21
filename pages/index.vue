<template>
  <!-- <v-progress-circular
      indeterminate
      color="primary"
  >
  </v-progress-circular> -->
  <Home :tweets="tweets" />
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
          name: 'Nikola Tesla',
          username: '@NikolaTesla',
          data: '7 de outubro',
          text: 'Inventor',
          subtitle: 'Nikola Tesla foi um inventor, engenheiro eletrotécnico'
        },
        {
          avatar: 'https://www3.unicentro.br/petfisica/wp-content/uploads/sites/54/2016/08/Tesla.jpg',
          name: 'Brunch this weekend?',
          username: '@qualquer',
          data: '4 de outubro',
          text: 'blablabla',
          subtitle: 'sdcfsdvfsddgfsd'
        },
        {
          avatar: 'https://www.nobelprize.org/images/einstein-12923-portrait-medium.jpg',
          name: 'Albert Einstein',
          username: '@Albert Einstein',
          data: '14 de março de 1879',
          text: ' físico teórico alemão',
          subtitle: 'Albert Einstein foi um físico teórico alemão que desenvolveu a teoria da relatividade geral, um dos pilares da física moderna ao lado da mecânica'
        }
      ]
    }
  },
  components: {
    Home
  }
}
</script>
