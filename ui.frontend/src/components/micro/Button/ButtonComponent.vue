<template>
    <button id="idButton">
        {{ text }}
    </button>
</template>

<script>

export default {
  name: 'ButtonComponent',
  props: {
    text: {
      type: String,
      default: 'Placeholder'
    }
  }
}

</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Space+Mono&display=swap');

#idButton {
    width: 216px;
    height: 68px;
    background: #333333;
    color: #FFFFFF;
    font-family: 'Space Mono';
    text-transform: uppercase;
    font-weight: 700;
    font-size: 14px;
}

</style>
