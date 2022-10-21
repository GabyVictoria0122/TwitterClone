<template>
  <h1>Aqui vai ser a timeline de um usuario chamado(a) {{ username }}</h1>
</template>

<script>
export default {
  name: 'IndexUser',
  asyncData (context) {
    console.log('Aqui é o context', context)
    return {
      username: context.params.username
    }
  }
}
</script>
