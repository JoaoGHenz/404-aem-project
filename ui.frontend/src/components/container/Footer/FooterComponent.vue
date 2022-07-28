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
  position: absolute;
  width: 99vw;
  bottom: 0px;
  //left: 96px;
  p {
    margin: 0;
  }
  @media (max-width: 768px)  {
      //a
    }
}

</style>
