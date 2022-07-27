<template>
    <header>
        <TitleComponent :text="textHeader" type="h1" titleClass="header" />
    </header>
</template>

<script>
import TitleComponent from '../../micro/Title/TitleComponent.vue'

export default {
  name: 'HeaderComponent',
  components: {
    TitleComponent
  },
  props: {
    textHeader: {
      type: String
    }
    /* classHeader: {
      type: String
    } */
  }
}

</script>

<style lang="scss" scoped>

</style>
