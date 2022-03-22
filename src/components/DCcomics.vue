<template>
<header>
    <div class="container">
        <img src="../../src/assets/img/dc-logo.png" alt="DC logo">
    <ul>
        <li v-for="element in links" :key="element"><a :href="element.href">{{ element.text }}</a></li>
    </ul>
    </div>
</header>
</template>
<script>
export default {
  name: 'DCcomics',
  data () {
    return {
      links: [
        {
          href: '#',
          text: 'characters'
        },
        {
          href: '#',
          text: 'comics'
        },
        {
          href: '#',
          text: 'movies'
        },
        {
          href: '#',
          text: 'tv'
        },
        {
          href: '#',
          text: 'games'
        },
        {
          href: '#',
          text: 'collectibles'
        },
        {
          href: '#',
          text: 'videos'
        },
        {
          href: '#',
          text: 'fans'
        },
        {
          href: '#',
          text: 'news'
        },
        {
          href: '#',
          text: 'shop'
        }
      ]
    }
  }
}
</script>

<style scoped lang='scss'>
.container{
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: red;
    padding: 1rem;
}

li {
    display: inline-block;
    margin: 0 0.5rem;
    text-transform: uppercase;
    a {
        text-decoration: none;
        color: black;
        padding-bottom: 3rem;
        border-bottom: 10px solid blue;

        &hover{

        }
    }
}

</style>
