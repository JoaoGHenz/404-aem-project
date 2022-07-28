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

#mainText {
    font-family: 'Space Mono';
    font-style: normal;
    font-weight: 400;
    font-size: 24px;
    color: #4F4F4F;
    width: 60%;

    @media (max-width: 768px) {
    font-size: 18px;
    line-height: 27px;
   }
}
</style>
