<template>
    <h1 :clas="titleClass" v-if="type === 'h1'">{{ text }}</h1>
    <h2 :clas="titleClass" v-else-if="type === 'h2'">{{ text }}</h2>
    <h3 :clas="titleClass" v-else-if="type === 'h3'">{{ text }}</h3>
    <h4 :clas="titleClass" v-else-if="type === 'h4'">{{ text }}</h4>
    <h5 :clas="titleClass" v-else-if="type === 'h5'">{{ text }}</h5>
    <h6 :clas="titleClass" v-else-if="type === 'h5'">{{ text }}</h6>
</template>

<script>

export default {
  name: 'TitleComponent',
  props: {
    titleClass: {
      type: String
    },
    type: {
      type: String,
      default: 'h2'
    },
    text: {
      type: String
    }
  }
}

</script>

<style scoped lang="scss">

</style>
