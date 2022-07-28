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

header {
  display: flex;
  justify-content: flex-start;
  align-items: flex-start;
  width: 90%;
  .header {
    margin: 0 0 10%;
    @media (max-width: 768px)  {
      margin: 0 0 5%;
    }
  }
}

</style>
