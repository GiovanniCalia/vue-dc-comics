<template>
<main>
    <div class="first-main">
      <div class="container">
        <h1>--> Content goes here --></h1>
      </div>
    </div>

    <div class="second-main">
      <div class="container">
        <ul class="ul-images">
          <li class="li-inline-block" v-for="element in links" :key="element" ><a :href="element.href">
            <img :src="element.img" :alt="element.text">
            <div>{{ element.text }}</div>
          </a></li>
        </ul>
      </div>
    </div>

    <div class="third-main">
      <div class="container float">
        <div class="little-container">
          <ul class="ul-second-main">
            <h2>dc comics</h2>
            <li class="second-li" v-for="element in DCcomicsLinks" :key="element"><a :href="element.href">
              <div>{{ element.text}}</div>
            </a></li>

            <h2>shop</h2>
            <li class="second-li" v-for="element in shopLinks" :key="element"><a :href="element.href">
              <div>{{ element.text}}</div>
            </a></li>
          </ul>
          <ul class="ul-second-main">
            <h2>dc</h2>
            <li class="second-li" v-for="element in DCLinks" :key="element"><a :href="element.href">
              <div>{{ element.text}}</div>
            </a></li>
          </ul>
          <ul class="ul-second-main">
            <h2>sites</h2>
            <li class="second-li" v-for="element in sites" :key="element"><a :href="element.href">
              <div>{{ element.text}}</div>
            </a></li>
          </ul>
        </div>
      </div>
    </div>
</main>

</template>

<script>
export default {
  name: 'mainDCcomics',
  data () {
    return {
      links: [
        {
          href: '#',
          img: '../../src/assets/img/buy-comics-digital-comics.png',
          text: 'digital comics'
        },
        {
          href: '#',
          img: '../../src/assets/img/buy-comics-merchandise.png',
          text: 'dc merchandise'
        },
        {
          href: '#',
          img: '../../src/assets/img/buy-comics-subscriptions.png',
          text: 'subscription'
        },
        {
          href: '#',
          img: '../../src/assets/img/buy-comics-locator.png',
          text: 'comic shop locator'
        },
        {
          href: '#',
          img: '../../src/assets/img/<svg version="1.1" id="Layer_2_1_" xmlns="http://www.w3.org/2000/svg" x="0" y="0" viewBox="0 0 79.5 50.9" xml:space="preserve"><style>.st0{fill:none;stroke:#fff;stroke-width:1.7732;stroke-miterlimit:10}</style><path class="st0" d="M73.9 49.6H5.3c-2.1 0-3.8-1.7-3.8-3.8V5.4c0-2.1 1.7-3.8 3.8-3.8h68.6c2.1 0 3.8 1.7 3.8 3.8v40.3c0 2.1-1.7 3.9-3.8 3.9zM1.5 15.4h76.2"/><path fill="#fff" stroke="#fff" stroke-width=".998" stroke-linecap="round" stroke-linejoin="round" stroke-miterlimit="10" d="M50.1 22.1l-9.7 1.4 5.1-16.4L29 30.2l9.3-1.3L34.4 44z"/></svg>',
          text: 'dc power visa'
        }
      ],
      DCcomicsLinks: [
        {
          href: '#',
          text: 'Characters'
        },
        {
          href: '#',
          text: 'Comics'
        },
        {
          href: '#',
          text: 'Movies'
        },
        {
          href: '#',
          text: 'TV'
        },
        {
          href: '#',
          text: 'Games'
        },
        {
          href: '#',
          text: 'Videos'
        },
        {
          href: '#',
          text: 'News'
        }
      ],
      shopLinks: [
        {
          href: '#',
          text: 'Shop DC'
        },
        {
          href: '#',
          text: 'Shop DC collectibles'
        }
      ],
      DCLinks: [
        {
          href: '#',
          text: 'Terms of use'
        },
        {
          href: '#',
          text: 'Privacy policy (New)'
        },
        {
          href: '#',
          text: 'Ad Choices'
        },
        {
          href: '#',
          text: 'Advertising'
        },
        {
          href: '#',
          text: 'Jobs'
        },
        {
          href: '#',
          text: 'Subscriptions'
        },
        {
          href: '#',
          text: 'Talent Workshops'
        },
        {
          href: '#',
          text: 'CPSC Certificates'
        },
        {
          href: '#',
          text: 'Ratings'
        },
        {
          href: '#',
          text: 'Shop Help'
        },
        {
          href: '#',
          text: 'Contact Us'
        }
      ],
      sites: [
        {
          href: '#!',
          text: 'DC'
        },
        {
          href: '#!',
          text: 'MAD Magazine'
        },
        {
          href: '#!',
          text: 'DC Kids'
        },
        {
          href: '#!',
          text: 'DC Universe'
        },
        {
          href: '#!',
          text: 'DC Power visa'
        }
      ]
    }
  }
}
</script>

<style scoped lang='scss'>
main{
  background-image: url(../../src/assets/img/footer-bg.jpg);
  background-size: cover;
}

.little-container{
  width: 600px;
}

.ul-second-main{
  float: left;
  margin: 2rem;
}

.float:after{
    content: "";
    display: table;
    clear: both;
}

.first-main{
  background-color: black;
}

.second-main{
  background-color: rgb(0, 130, 249);
}

.ul-images {
  text-align: center;
}

h1{
  color: white;
  line-height: 8rem;
}

.li-inline-block{
  display: inline-block;
  margin: 2rem;

  a{
    text-transform: uppercase;
    text-decoration: none;
    color: white;
  }
}

h2 {
  text-transform: uppercase;
  margin-bottom: 1rem;
  color: white;
  margin-top: 1rem;
}

.second-li{
  list-style-type: none;
  margin-bottom: 5px;

  a{
  text-decoration: none;
  color: grey;
}
}

</style>
