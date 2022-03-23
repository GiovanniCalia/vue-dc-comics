<template>
<header>
    <div class="container">
        <img src="../../src/assets/img/dc-logo.png" alt="DC logo">
    <ul>
        <li @click='setActiveIndex(index)' v-for="(element,index) in links" :key="element" :class="{active: index == activeIndex}"><a :href="element.href">{{ element.text }}</a></li>
    </ul>
    </div>
</header>
</template>
<script>
export default {
  name: 'DCcomics',
  data () {
    return {
      activeIndex: 1,
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
  },
  methods: {
    setActiveIndex (index) {
      this.activeIndex = index
    }
  }
}
</script>

<style scoped lang='scss'>
@import '@/assets/styles/otherstyles/variables.scss';

.container{
    display: flex;
    align-items: center;
    justify-content: space-between;
}

img{
  width: 8%;
}

li {
    display: inline-block;
    margin: 0 0.5rem;
    text-transform: uppercase;

    &.active{
      line-height: 8rem;
      border-bottom: 7px solid $blue_color;
    }

    a {
        text-decoration: none;
        color: black;

    }
}

</style>
