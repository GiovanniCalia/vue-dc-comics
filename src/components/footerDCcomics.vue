<template>
  <footer>
      <div class="container">
        <div class="btn">sign up now!</div>
        <div class="images">
          <div>follow us</div>
          <img src="../../src/assets/img/footer-facebook.png" alt="">
          <img src="../../src/assets/img/footer-twitter.png" alt="">
          <img src="../../src/assets/img/footer-youtube.png" alt="">
          <img src="../../src/assets/img/footer-pinterest.png" alt="">
          <img src="../../src/assets/img/footer-periscope.png" alt="">
        </div>
      </div>
  </footer>
</template>

<script>
export default {
  name: 'footerDCcomics'
}
</script>

<style scoped lang='scss'>
footer{
  background-color: rgb(48, 48, 48);
}
.container{
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.btn{
  text-transform: uppercase;
  padding: 0.8rem;
  color: white;
  background-color: transparent;
  border: 2px solid rgb(0, 130, 249);

  &:hover{
    cursor: pointer;
  }
}
.images{
  display: flex;
  align-items: center;

  div{
    text-transform: uppercase;
    color: rgb(0, 130, 249);
    line-height: 5rem;
    margin-right: 2rem;

    &:hover{
      cursor: pointer;
    }
  }

  img{
    margin-right: 1rem;
  }
}
</style>
