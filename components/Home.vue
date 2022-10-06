<template>
  <Timeline :tweets="tweets" />
</template>

<script>
import Timeline from '../components/Timeline.vue'

export default {
  name: 'HomePage',
  props: ['tweets'],
  components: {
    Timeline
  }
}
</script>
