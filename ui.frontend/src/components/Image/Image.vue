<template>
  <img :src="src" />
</template>

<script>
export default {
  name: 'Image',
  props: {
    src: {
      type: String
    }
  }
}
</script>

<style scoped>
img {
  max-width: 40vw;
}

@media (max-width: 768px) {
  img {
    max-width: 60vw;
  }
}
</style>
