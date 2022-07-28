<template>
    <h1 :class="titleClass" v-if="type === 'h1'">{{ text }}</h1>
    <h2 :class="titleClass" v-else-if="type === 'h2'">{{ text }}</h2>
    <h3 :class="titleClass" v-else-if="type === 'h3'">{{ text }}</h3>
    <h4 :class="titleClass" v-else-if="type === 'h4'">{{ text }}</h4>
    <h5 :class="titleClass" v-else-if="type === 'h5'">{{ text }}</h5>
    <h6 :class="titleClass" v-else-if="type === 'h6'">{{ text }}</h6>
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

<style lang="scss" scoped>

@import url('https://fonts.googleapis.com/css2?family=Inconsolata&display=swap');

.header {
    font-family: 'Inconsolata';
    font-style: normal;
    font-weight: 700;
    font-size: 24px;
}

.mainTitle {
    font-family: 'Space Mono';
    font-style: normal;
    font-weight: 700;
    font-size: 64px;
    color: #333333;
    margin: 0;
}

</style>
