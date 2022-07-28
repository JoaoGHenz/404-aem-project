<template>
    <footer class="footer">
        <p class="footerTitle">created by {{ username }} - {{ company }}</p>
    </footer>
</template>

<script>

export default {
  name: 'FooterComponent',
  props: {
    username: {
      type: String
    },
    company: {
      type: String,
      default: 'compass.uol'
    }
  }
}

</script>

<style lang="scss" scoped>

@import url('https://fonts.googleapis.com/css2?family=Montserrat&display=swap');

.footer {
  font-family: 'Montserrat';
  font-weight: 500;
  font-size: 14px;
  color: #BDBDBD;
  text-align: center;
  margin: 5% 0 0;
  p {
    margin: 0;
  }
  @media (max-width: 768px)  {
      margin: 2% 0 0;
    }
}

</style>
