<template>
    <header>
        <TitleComponent :text="textHeader" type="h1" :titleClass="classHeader" />
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
    },
    classHeader: {
      type: String
    }
  }
}

</script>

<style>

</style>
