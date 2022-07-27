<template>
    <p :id="idText">{{ text }}</p>
</template>

<script>
export default {
  name: 'TextComponent',
  props: {
    text: {
      type: String
    },
    idText: {
      type: String
    }
  }
}

</script>

<style scoped lang="scss">
#basicText {
    font-size: 1.5em;
}
</style>
