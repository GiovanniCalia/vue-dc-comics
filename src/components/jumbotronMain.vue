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
@import '@/assets/styles/otherstyles/variables.scss';

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
  font-size: 1.5rem;
  color: white;
  background-color: $blue_color;
  border: none;
  text-transform: uppercase;
  position: absolute;
  bottom: 0;
  left: 0;
  margin-bottom: calc(-37.89px / 2);

  &:hover{
    cursor: pointer;
  }
}

</style>
