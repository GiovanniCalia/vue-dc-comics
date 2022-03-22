<template>
<header>
    <img src="../../src/assets/img/dc-logo.png" alt="DC logo">
    <ul>
        <li v-for="element in links" :key="element"><a :href="element.href">{{ element.text }}</a></li>
    </ul>
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
