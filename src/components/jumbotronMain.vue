<template>
  <main>
    <div class="container">
      <button>current series</button>
    </div>
  </main>
</template>

<script>
export default {
  name: 'jumbotronMain'
}
</script>

<style scoped lang='scss'>
main{
  background-image: url(../../src/assets/img/jumbotron.jpg);
  background-size: cover;
  height: 300px;
}

.container{
  position: relative;
  height: 100%;
}

button{
  padding: 0.7rem;
  color: white;
  background-color: rgb(0, 130, 249);
  border: none;
  text-transform: uppercase;
  position: absolute;
  bottom: 0;
  left: 0;
  margin-bottom: calc(-37.89px / 2)
}

</style>
