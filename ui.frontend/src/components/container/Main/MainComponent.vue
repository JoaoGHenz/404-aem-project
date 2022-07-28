<template>

    <main>
        <TitleComponent titleClass="mainTitle" type="h2" :text="titleText" />
        <TextComponent idText="mainText" :text="textText" />
        <ButtonComponent :text="buttonText" />
    </main>

</template>

<script>
import TitleComponent from '../../micro/Title/TitleComponent'
import TextComponent from '../../micro/Text/TextComponent'
import ButtonComponent from '../../micro/Button/ButtonComponent'

export default {
  name: 'MainComponent',
  components: {
    TitleComponent,
    TextComponent,
    ButtonComponent
  },
  props: {
    titleText: {
      type: String
    },
    textText: {
      type: String
    },
    buttonText: {
      type: String
    }
  }

}

</script>

<style lang="scss" scoped>

main {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  display: flex;
  flex-flow: column wrap;
  justify-content: space-around;
}

</style>
